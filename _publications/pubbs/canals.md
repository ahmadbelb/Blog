---
title: "Hello canals in Southeast Asian peatlands increase carbon emissions"
collection: publications
permalink: /publication/canals
excerpt: 'This paper presents a novel convolutional neural network to detect canals and study the effect of canals on land subsidence.'
date: 2021-03-23
venue: 'AGU Advances'
paperurl: 'https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020AV000321'
citation: 'Dadap, N. C., Hoyt, A. M., Cobb, A. R., Oner, D., Kozinski, M., Fua, P. V., <b>Rao, K.</b>, Harvey, C. F., & Konings, A. G. (2021). Drainage Canals in Southeast Asian Peatlands Increase Carbon Emissions. AGU Advances, 2(1), e2020AV000321. https://doi.org/10.1029/2020AV000321'
---

Tropical peatlands are swamp‐like environments in which naturally wet conditions slow the decomposition of plant carbon that would otherwise be released to the atmosphere. However, over the past few decades, humans have built drainage canals in Southeast Asian peatlands, due to economic pressure for logging and agriculture. These canals are a major threat to peatlands because they dry out peat soils, in turn speeding up decomposition and making soils susceptible to wildfire. Both of these mechanisms release massive amounts of carbon dioxide to the atmosphere, thereby accelerating climate change. Despite these risks, until now the extent of drainage in peatlands was unknown due to a lack of drainage canal maps. Here, we create the first regional map of drainage canals by training a computer algorithm to identify canals within high‐resolution satellite images. We find that drainage is widespread—occurring in at least 65% of Southeast Asian peatlands. Furthermore, we find that more drainage canals are related to progressively larger subsidence rates—deformations in the ground surface partly caused by carbon dioxide emissions to the atmosphere. These findings suggest that it is important to know where and how much drainage is occurring to accurately predict subsidence and target areas for restoration.

q


_Canal segmentation results_
```
conditions
{
    Is Dummy Bot(Event Player) == False;
}
```

{% capture code %}{% raw %}variables
{
    player:
        100: directionString
        101: wasdString
        102: jumpIndicator
        103: showWASD
        104: wasdCollector
}

rule("HUD -------------------------------------------------- WASD / Space Indicators for Spec")
{
    event
    {
        Ongoing - Each Player;
        All;
        All;
    }

    conditions
    {
        Is Communicating Any Spray(Event Player) == True;
        disabled Is Button Held(Event Player, Button(Ultimate)) == True;
    }

    actions
    {
        If(Event Player.showWASD == False);
            Event Player.jumpIndicator = Custom String("            ");
            Event Player.wasdCollector = Array();
            Create HUD Text(Event Player, Event Player.jumpIndicator, Null, Null, Top, -46, Color(White), Color(White), Color(White),
                Visible To and String, Default Visibility);
            Modify Player Variable(Event Player, wasdCollector, Append To Array, Last Text ID);
            Create HUD Text(Event Player, Event Player.wasdString, Null, Null, Top, -46, Color(White), Color(White), Color(White),
                Visible To and String, Default Visibility);
            Modify Player Variable(Event Player, wasdCollector, Append To Array, Last Text ID);
            disabled Create HUD Text(Event Player, Event Player.directionString, Null, Null, Top, -46, Color(White), Color(White), Color(White),
                Visible To and String, Default Visibility);
            disabled Modify Player Variable(Event Player, wasdCollector, Append To Array, Last Text ID);
            Event Player.showWASD = True;
        Else;
            Destroy HUD Text(Event Player.wasdCollector[0]);
            Destroy HUD Text(Event Player.wasdCollector[1]);
            Destroy HUD Text(Event Player.wasdCollector[2]);
            Event Player.showWASD = False;
    }
}

rule("Check for direction ------------------------------ WASD / Space Indicators for Spec")
{
    event
    {
        Ongoing - Each Player;
        All;
        All;
    }

    conditions
    {
        Event Player.showWASD == True;
    }

    actions
    {
        "Forward"
        If(Z Component Of(Throttle Of(Event Player)) == 1 && X Component Of(Throttle Of(Event Player)) == 0);
            Event Player.directionString = Custom String("     ·     \n           \n           ");
            Event Player.wasdString = Custom String(" _↑_ _ ");
        "Backwards"
        Else If(Z Component Of(Throttle Of(Event Player)) == -1 && X Component Of(Throttle Of(Event Player)) == 0);
            Event Player.directionString = Custom String("           \n           \n     ·     ");
            Event Player.wasdString = Custom String(" _ _↓_ ");
        "Left"
        Else If(Z Component Of(Throttle Of(Event Player)) == 0 && X Component Of(Throttle Of(Event Player)) == 1);
            Event Player.directionString = Custom String("           \n  ·        \n           ");
            Event Player.wasdString = Custom String("←_ _ _ ");
        "Right"
        Else If(Z Component Of(Throttle Of(Event Player)) == 0 && X Component Of(Throttle Of(Event Player)) == -1);
            Event Player.directionString = Custom String("           \n        ·  \n           ");
            Event Player.wasdString = Custom String(" _ _ _→");
        "Forward Left"
        Else If(Z Component Of(Throttle Of(Event Player)) == 1 && X Component Of(Throttle Of(Event Player)) == 1);
            Event Player.directionString = Custom String("  ·        \n           \n           ");
            Event Player.wasdString = Custom String("←↑_ _ ");
        "Forward Right"
        Else If(Z Component Of(Throttle Of(Event Player)) == 1 && X Component Of(Throttle Of(Event Player)) == -1);
            Event Player.directionString = Custom String("        ·  \n           \n           ");
            Event Player.wasdString = Custom String(" _↑_→");
        "Backwards Left"
        Else If(Z Component Of(Throttle Of(Event Player)) == -1 && X Component Of(Throttle Of(Event Player)) == 1);
            Event Player.directionString = Custom String("           \n           \n  ·        ");
            Event Player.wasdString = Custom String("←_↓_ ");
        "Backwards Right"
        Else If(Z Component Of(Throttle Of(Event Player)) == -1 && X Component Of(Throttle Of(Event Player)) == -1);
            Event Player.directionString = Custom String("           \n           \n        ·  ");
            Event Player.wasdString = Custom String(" _ _↓→");
        "No input"
        Else If(Z Component Of(Throttle Of(Event Player)) == 0 && X Component Of(Throttle Of(Event Player)) == 0);
            Event Player.directionString = Custom String("           \n     ·     \n           ");
            Event Player.wasdString = Custom String(" _ _ _ _ ");
        End;
        Wait(Update Every Frame(Throttle Of(Event Player)), Ignore Condition);
        Loop If Condition Is True;
    }
}

rule("Check for space ---------------------------------- WASD / Space Indicators for Spec")
{
    event
    {
        Ongoing - Each Player;
        All;
        All;
    }

    conditions
    {
        Is Button Held(Event Player, Button(Jump)) == True;
        Event Player.showWASD == True;
    }

    actions
    {
        Event Player.jumpIndicator = Custom String("SPACE");
        Wait Until(!Is Button Held(Event Player, Button(Jump)), 99999);
        Event Player.jumpIndicator = Custom String("             ");
    }
}{% endraw %}{% endcapture %}  
{% include code.html code=code %}

<div class="highlight-default notranslate"><div class="highlight"><pre id="codecell1"><span></span><span class="n">jupyter</span> <span class="n">nbconvert</span> <span class="n">github_page_example</span><span class="o">.</span><span class="n">ipynb</span> <span class="o">--</span><span class="n">to</span> <span class="n">slides</span> <span class="o">--</span><span class="n">stdout</span> <span class="o">&gt;</span> <span class="n">index</span><span class="o">.</span><span class="n">html</span>
</pre><a class="copybtn o-tooltip--left" style="background-color: rgb(250, 250, 250)" data-tooltip="Copy" data-clipboard-target="#codecell1">
      <img src="https://ahmadbelb.github.io/Blog/images/copy-button.svg" alt="Copy to clipboard">
    </a></div>
</div>

<style>
table, tr, td ,th{
   border: none!important;
}
</style>

<hr>
<body class="sponsored">

<h2 class="centered"> Research graciously funded by</h2>

<table >
  <tr >
    <td ><a class="greyed" href="https://www.eng.ed.ac.uk/" target="_blank"> <img src="https://ahmadbelb.github.io/Blog/images/ed.png"  alt="1" width = 500px ></a></td>

    <td><a class="greyed" href="https://www.Arup.com/" target="_blank"><img src="https://ahmadbelb.github.io/Blog/images/Arup.png" alt="2" width = 360px ></a></td>
 <td><a class="greyed" href="https://www.transport.gov.scot/" target="_blank"><img src="https://ahmadbelb.github.io/Blog/images/scot.png" alt="2" width = 400px ></a></td>
   </tr> 
   <tr>
    

     
  </tr>
</table>
</body>

