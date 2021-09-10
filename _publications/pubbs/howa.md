---
title: "APDL modal TEST "
excerpt: "Map is a <br/><img src='https://ahmadbelb.github.io/Blog/images/modal1.gif' Width= 876px Height= 480px  loop=infinite>"
collection: publications
permalink: /publication/howa
date: 2021-03-23
venue: 'AGU Advances'
paperurl: ''
citation: ''
---

# How to QA

This template explains our QA process for shipping bug-free software.

# QA Philosophy

Write about your approach to QA and why it's critical to success. 

# Processes

### Making Code Changes

- Test PRs rigorously before requesting review.
- Include test cases you've checked for in your PR description.

### Reviewing Code

- If the change is substantial and user-facing, pull down the branch.
- Test for cases (particularly edge cases) that the PR author may have missed.

### QA

- Look at the list of items going out for release the next day.
- Go down the list one-by-one and thoroughly test changes.

```fortran
/INPUT FILE= C:\Users\PAPERS~1\AppData\Local\Temp\tmp_iematbmcia.inp  LINE=       0
 --- Data in consistent MKS units. See Solving Units in the help system for more

 MKS UNITS SPECIFIED FOR INTERNAL    
  LENGTH        (l)  = METER (M)
  MASS          (M)  = KILOGRAM (KG)
  TIME          (t)  = SECOND (SEC)
  TEMPERATURE   (T)  = CELSIUS (C)
  TOFFSET            = 273.0
  CHARGE        (Q)  = COULOMB
  FORCE         (f)  = NEWTON (N) (KG-M/SEC2)
  HEAT               = JOULE (N-M)

  PRESSURE           = PASCAL (NEWTON/M**2)
  ENERGY        (W)  = JOULE (N-M)
  POWER         (P)  = WATT (N-M/SEC)
  CURRENT       (i)  = AMPERE (COULOMBS/SEC)
  CAPACITANCE   (C)  = FARAD
  INDUCTANCE    (L)  = HENRY
  MAGNETIC FLUX      = WEBER
  RESISTANCE    (R)  = OHM
  ELECTRIC POTENTIAL = VOLT

 INPUT  UNITS ARE ALSO SET TO MKS 

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:08  SEP 10, 2021 CP=      0.422

                                                                               

          ***** ANSYS ANALYSIS DEFINITION (PREP7) *****
 *********** Nodes for the whole assembly ***********
 *********** Elements for Body 1 "Solid" ***********
 *********** Send User Defined Coordinate System(s) ***********
 *********** Set Reference Temperature ***********
 *********** Send Materials ***********
 *********** Fixed Supports ***********
 ******* Constant Zero Displacement Y *******
 ******* Constant Zero Displacement Z *******
 *********** Define Pressure Using Surface Effect Elements "Pressure" **********

 ***** ROUTINE COMPLETED *****  CP =         0.438

 --- Number of total nodes = 849
 --- Number of contact elements = 80
 --- Number of spring elements = 0
 --- Number of bearing elements = 0
 --- Number of solid elements = 120
 --- Number of condensed parts = 0
 --- Number of total elements = 200

 *GET  _WALLBSOL  FROM  ACTI  ITEM=TIME WALL  VALUE=  11.1522222    
 ****************************************************************************
 *************************    SOLUTION       ********************************
 ****************************************************************************

 *****  ANSYS SOLUTION ROUTINE  *****

 PERFORM A STATIC ANALYSIS
  THIS WILL BE A NEW ANALYSIS

 PARAMETER _THICKRATIO =     0.000000000    

 USE SPARSE MATRIX DIRECT SOLVER

 CONTACT INFORMATION PRINTOUT LEVEL       1

 NLDIAG: Nonlinear diagnostics CONT option is set to ON. 
         Writing frequency : each ITERATION.

 DO NOT SAVE ANY RESTART FILES AT ALL
 ****************************************************
 ******************* SOLVE FOR LS 1 OF 1 ****************

 SELECT       FOR ITEM=TYPE COMPONENT=    
  IN RANGE         2 TO          2 STEP          1

         80  ELEMENTS (OF        200  DEFINED) SELECTED BY  ESEL  COMMAND.

 SELECT      ALL NODES HAVING ANY ELEMENT IN ELEMENT SET.

        289 NODES (OF        849  DEFINED) SELECTED FROM
       80 SELECTED ELEMENTS BY NSLE COMMAND.

 GENERATE SURFACE LOAD PRES ON SURFACE DEFINED BY ALL SELECTED NODES
 VALUES=  150.000000      0.00000000    

 NUMBER OF PRES ELEMENT FACE LOADS STORED =         80

 ALL SELECT   FOR ITEM=NODE COMPONENT=    
  IN RANGE         1 TO        849 STEP          1

        849  NODES (OF        849  DEFINED) SELECTED BY NSEL  COMMAND.

 ALL SELECT   FOR ITEM=ELEM COMPONENT=    
  IN RANGE         1 TO        452 STEP          1

        200  ELEMENTS (OF        200  DEFINED) SELECTED BY  ESEL  COMMAND.

 ALL SELECT   FOR ITEM=ELEM COMPONENT=    
  IN RANGE         1 TO        452 STEP          1

        200  ELEMENTS (OF        200  DEFINED) SELECTED BY  ESEL  COMMAND.

 PRINTOUT RESUMED BY /GOP

 USE       1 SUBSTEPS INITIALLY THIS LOAD STEP FOR ALL  DEGREES OF FREEDOM
 FOR AUTOMATIC TIME STEPPING:
   USE      1 SUBSTEPS AS A MAXIMUM
   USE      1 SUBSTEPS AS A MINIMUM

 TIME=  1.0000    

 ERASE THE CURRENT DATABASE OUTPUT CONTROL TABLE.

 WRITE ALL  ITEMS TO THE DATABASE WITH A FREQUENCY OF NONE
   FOR ALL APPLICABLE ENTITIES

 WRITE NSOL ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE RSOL ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE EANG ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE ETMP ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE VENG ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE STRS ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE EPEL ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE EPPL ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE CONT ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 *GET  ANSINTER_  FROM  ACTI  ITEM=INT        VALUE=  0.00000000    

 *IF  ANSINTER_                         ( =   0.00000     )  NE  
      0                                 ( =   0.00000     )  THEN    

 *ENDIF

 *****  ANSYS SOLVE    COMMAND  *****

 *** NOTE ***                            CP =       0.438   TIME= 11:09:08
 There is no title defined for this analysis.                            

 *** SELECTION OF ELEMENT TECHNOLOGIES FOR APPLICABLE ELEMENTS ***
      --- GIVE SUGGESTIONS AND RESET THE KEY OPTIONS ---

 ELEMENT TYPE         1 IS SOLID186. KEYOPT(2)=0 IS SUGGESTED AND HAS BEEN RESET.
  KEYOPT(1-12)=    0    0    0    0    0    0    0    0    0    0    0    0

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:08  SEP 10, 2021 CP=      0.438

                                                                               

                       S O L U T I O N   O P T I O N S

   PROBLEM DIMENSIONALITY. . . . . . . . . . . . .3-D                  
   DEGREES OF FREEDOM. . . . . . UX   UY   UZ  
   ANALYSIS TYPE . . . . . . . . . . . . . . . . .STATIC (STEADY-STATE)
   OFFSET TEMPERATURE FROM ABSOLUTE ZERO . . . . .  273.15    
   EQUATION SOLVER OPTION. . . . . . . . . . . . .SPARSE             
   GLOBALLY ASSEMBLED MATRIX . . . . . . . . . . .SYMMETRIC  

 *** WARNING ***                         CP =       0.438   TIME= 11:09:08
 Material number 2 (used by element 373) should normally have at least   
 one MP or one TB type command associated with it.  Output of energy by  
 material may not be available.                                          

 *** NOTE ***                            CP =       0.438   TIME= 11:09:08
 The step data was checked and warning messages were found.              
  Please review output or errors file (                                  
 C:\Users\PAPERS~1\AppData\Local\Temp\ansys_etlukvhxzp\file.err ) for    
 these warning messages.                                                 

 *** NOTE ***                            CP =       0.438   TIME= 11:09:08
 The conditions for direct assembly have been met.  No .emat or .erot    
 files will be produced.                                                 

                      L O A D   S T E P   O P T I O N S

   LOAD STEP NUMBER. . . . . . . . . . . . . . . .     1
   TIME AT END OF THE LOAD STEP. . . . . . . . . .  1.0000    
   NUMBER OF SUBSTEPS. . . . . . . . . . . . . . .     1
   STEP CHANGE BOUNDARY CONDITIONS . . . . . . . .    NO
   PRINT OUTPUT CONTROLS . . . . . . . . . . . . .NO PRINTOUT
   DATABASE OUTPUT CONTROLS
      ITEM     FREQUENCY   COMPONENT
       ALL       NONE               
      NSOL        ALL               
      RSOL        ALL               
      EANG        ALL               
      ETMP        ALL               
      VENG        ALL               
      STRS        ALL               
      EPEL        ALL               
      EPPL        ALL               
      CONT        ALL               

 SOLUTION MONITORING INFO IS WRITTEN TO FILE= file.mntr                                                                                                                                                                                                                                                           

                         ***********  PRECISE MASS SUMMARY  ***********

   TOTAL RIGID BODY MASS MATRIX ABOUT ORIGIN
               Translational mass               |   Coupled translational/rotational mass
         1178.2        0.0000        0.0000     |     0.0000        1413.9       -76.485    
         0.0000        1178.2        0.0000     |    -1413.9        0.0000        1.0669    
         0.0000        0.0000        1178.2     |     76.485       -1.0669        0.0000    
     ------------------------------------------ | ------------------------------------------
                                                |         Rotational mass (inertia)
                                                |     2268.3      -0.88451E-01   -1.2803    
                                                |   -0.88451E-01    2280.4       -91.782    
                                                |    -1.2803       -91.782        24.283    

   TOTAL MASS =  1178.2    
     The mass principal axes coincide with the global Cartesian axes

   CENTER OF MASS (X,Y,Z)=   0.90553E-03   0.64915E-01    1.2000    

   TOTAL INERTIA ABOUT CENTER OF MASS
         566.72      -0.19192E-01   0.42346E-13
       -0.19192E-01    583.70       0.14160E-11
        0.42346E-13   0.14160E-11    19.317    
     The inertia principal axes coincide with the global Cartesian axes

  *** MASS SUMMARY BY ELEMENT TYPE ***

  TYPE      MASS
     1   1178.23    

 Range of element maximum matrix coefficients in global coordinates
 Maximum = 3.422327942E+10 at element 20.                                
 Minimum = 2.893115481E+10 at element 72.                                

   *** ELEMENT MATRIX FORMULATION TIMES
     TYPE    NUMBER   ENAME      TOTAL CP  AVE CP

        1       120  SOLID186      0.125   0.001042
        2        80  SURF154       0.125   0.001563
 Time at end of element matrix formulation CP = 0.515625.                

 SPARSE MATRIX DIRECT SOLVER.
  Number of equations =        2402,    Maximum wavefront =    177
  Memory allocated for solver              =     7.269 MB
  Memory required for in-core solution     =     7.023 MB
  Memory required for out-of-core solution =     4.506 MB

 *** NOTE ***                            CP =       0.750   TIME= 11:09:08
 The Sparse Matrix Solver is currently running in the in-core memory     
 mode.  This memory mode uses the most amount of memory in order to      
 avoid using the hard drive as much as possible, which most often        
 results in the fastest solution time.  This mode is recommended if      
 enough physical memory is present to accommodate all of the solver      
 data.                                                                   
 curEqn=   2402  totEqn=   2402 Job CP sec=      0.875
      Factor Done= 100% Factor Wall sec=      0.000 rate=       0.0 Mflops
 Sparse solver maximum pivot= 5.244085573E+10 at node 543 UY.            
 Sparse solver minimum pivot= 108420946 at node 98 UX.                   
 Sparse solver minimum pivot in absolute value= 108420946 at node 98 UX. 

   *** ELEMENT RESULT CALCULATION TIMES
     TYPE    NUMBER   ENAME      TOTAL CP  AVE CP

        1       120  SOLID186      0.125   0.001042
        2        80  SURF154       0.000   0.000000

   *** NODAL LOAD CALCULATION TIMES
     TYPE    NUMBER   ENAME      TOTAL CP  AVE CP

        1       120  SOLID186      0.062   0.000521
        2        80  SURF154       0.062   0.000781
 *** LOAD STEP     1   SUBSTEP     1  COMPLETED.    CUM ITER =      1
 *** TIME =   1.00000         TIME INC =   1.00000      NEW TRIANG MATRIX

 *** ANSYS BINARY FILE STATISTICS
  BUFFER SIZE USED= 16384
        1.500 MB WRITTEN ON ASSEMBLED MATRIX FILE: file.full
        0.500 MB WRITTEN ON RESULTS FILE: file.rst
 *************** Write FE CONNECTORS *********

 WRITE OUT CONSTRAINT EQUATIONS TO FILE= file.ce                                                                                                                                                                                                                                                             
 ****************************************************
 *************** FINISHED SOLVE FOR LS 1 *************

 ALL CURRENT ANSYS DATA WRITTEN TO FILE NAME= file.db
  FOR POSSIBLE RESUME FROM THIS POINT

 *GET  _WALLASOL  FROM  ACTI  ITEM=TIME WALL  VALUE=  11.1522222    

 PRINTOUT RESUMED BY /GOP

 FINISH SOLUTION PROCESSING

 ***** ROUTINE COMPLETED *****  CP =         1.062

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:08  SEP 10, 2021 CP=      1.062

                                                                               

          ***** ANSYS RESULTS INTERPRETATION (POST1) *****

 *** NOTE ***                            CP =       1.062   TIME= 11:09:08
 Reading results into the database (SET command) will update the current 
 displacement and force boundary conditions in the database with the     
 values from the results file for that load set.  Note that any          
 subsequent solutions will use these values unless action is taken to    
 either SAVE the current values or not overwrite them (/EXIT,NOSAVE).    

 Set Encoding of XML File to:ISO-8859-1

 Set Output of XML File to:
     PARM,     ,     ,     ,     ,     ,     ,     ,     ,     ,     ,     ,
         ,     ,     ,     ,     ,     ,     ,

 DATABASE WRITTEN ON FILE  parm.xml                                                                                                                                                                                                                                                            

 EXIT THE ANSYS POST1 DATABASE PROCESSOR

 ***** ROUTINE COMPLETED *****  CP =         1.125

 PRINTOUT RESUMED BY /GOP

 *GET  _WALLDONE  FROM  ACTI  ITEM=TIME WALL  VALUE=  11.1522222    

 *** WARNING ***                         CP =       1.125   TIME= 11:09:08
 Unknown parameter name= _WALLSTRT.  A value of 7.888609052E-31 will be  
 used.                                                                   

 PARAMETER _PREPTIME =     40148.00000    

 PARAMETER _SOLVTIME =     0.000000000    

 PARAMETER _POSTTIME =     0.000000000    

 *** WARNING ***                         CP =       1.125   TIME= 11:09:08
 Unknown parameter name= _WALLSTRT.  A value of 7.888609052E-31 will be  
 used.                                                                   

 PARAMETER _TOTALTIM =     40148.00000    

 *GET  _DLBRATIO  FROM  ACTI  ITEM=SOLU DLBR  VALUE=  0.00000000    

 *GET  _COMBTIME  FROM  ACTI  ITEM=SOLU COMB  VALUE=  0.00000000    

 *GET  _SSMODE   FROM  ACTI  ITEM=SOLU SSMM  VALUE=  2.00000000    

 *GET  _NDOFS    FROM  ACTI  ITEM=SOLU NDOF  VALUE=  2402.00000    
 --- Total number of nodes = 849
 --- Total number of elements = 200
 --- Element load balance ratio = 0
 --- Time to combine distributed files = 0
 --- Sparse memory mode = 2
 --- Number of DOF = 2402

 ALL CURRENT ANSYS DATA WRITTEN TO FILE NAME= file.db
  FOR POSSIBLE RESUME FROM THIS POINT

 *GET  _WALLASOL  FROM  ACTI  ITEM=TIME WALL  VALUE=  11.1522222    

 PRINTOUT RESUMED BY /GOP

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:08  SEP 10, 2021 CP=      1.172

                                                                               

          ***** ANSYS RESULTS INTERPRETATION (POST1) *****

 Set Encoding of XML File to:ISO-8859-1

 Set Output of XML File to:
     PARM,     ,     ,     ,     ,     ,     ,     ,     ,     ,     ,     ,
         ,     ,     ,     ,     ,     ,     ,

 DATABASE WRITTEN ON FILE  parm.xml                                                                                                                                                                                                                                                            

 EXIT THE ANSYS POST1 DATABASE PROCESSOR

 ***** ROUTINE COMPLETED *****  CP =         1.172

 PRINTOUT RESUMED BY /GOP

 *GET  _WALLDONE  FROM  ACTI  ITEM=TIME WALL  VALUE=  11.1522222    

 *** WARNING ***                         CP =       1.172   TIME= 11:09:08
 Unknown parameter name= _WALLSTRT.  A value of 7.888609052E-31 will be  
 used.                                                                   

 PARAMETER _PREPTIME =     40148.00000    

 PARAMETER _SOLVTIME =     0.000000000    

 PARAMETER _POSTTIME =     0.000000000    

 *** WARNING ***                         CP =       1.172   TIME= 11:09:08
 Unknown parameter name= _WALLSTRT.  A value of 7.888609052E-31 will be  
 used.                                                                   

 PARAMETER _TOTALTIM =     40148.00000    

 *GET  _DLBRATIO  FROM  ACTI  ITEM=SOLU DLBR  VALUE=  0.00000000    

 *GET  _COMBTIME  FROM  ACTI  ITEM=SOLU COMB  VALUE=  0.00000000    

 *GET  _SSMODE   FROM  ACTI  ITEM=SOLU SSMM  VALUE=  2.00000000    

 *GET  _NDOFS    FROM  ACTI  ITEM=SOLU NDOF  VALUE=  2402.00000    
 --- Total number of nodes = 849
 --- Total number of elements = 200
 --- Element load balance ratio = 0
 --- Time to combine distributed files = 0
 --- Sparse memory mode = 2
 --- Number of DOF = 2402

 *** WARNING ***                         CP =       1.172   TIME= 11:09:08
 The /BATCH command must be the first line of input.  The /BATCH command 
 is ignored.                                                             

 DO NOT WRITE ELEMENT RESULTS INTO DATABASE

 *GET  _WALLSTRT  FROM  ACTI  ITEM=TIME WALL  VALUE=  11.1522222    

 ASSIGN FILE RSTP TO file.rst                                                                                                                                                                                                                                                            

 *****  ANSYS SOLUTION ROUTINE  *****

 PERFORM A STATIC ANALYSIS
  RESTART WILL BE PERFORMED FOR THE ANALYSIS OF LINEAR PERTURBATION
  RESTART WILL BE PERFORMED BASED ON: 
   PREVIOUS LOADSTEP =      1 SUBSTEP =      1

 *** ERROR ***                           CP =       1.359   TIME= 11:09:09
 During the multiframe restart process, neither the .RDB file nor the    
 .Rnnn file was found.  Both files are required to perform the           
 multiframe restart for the linear perturbation analysis.  You must use  
 the RESCONTROL,LINEAR command in the prior base analysis.  The          
 ANTYPE,,RESTART command is ignored.                                     
  ACT Extensions:
      LSDYNA, 2021.1
      5f463412-bd3e-484b-87e7-cbc0a665e474, wbex
  

 PERTURB: Enabling perturbation analysis with prestressed modal solution.
 PERTURB: Enabling perturbation contact status remains the same as in restart step.
 PERTURB: Enabling perturbation to delete all boundary conditions except for constraints and temperatures and also put all non-zero displacement constraints to zero values.

 *****  ANSYS SOLVE    COMMAND  *****

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:09  SEP 10, 2021 CP=      1.359

                                                                               

                       S O L U T I O N   O P T I O N S

   PROBLEM DIMENSIONALITY. . . . . . . . . . . . .3-D                  
   DEGREES OF FREEDOM. . . . . . UX   UY   UZ  
   ANALYSIS TYPE . . . . . . . . . . . . . . . . .STATIC (STEADY-STATE)
      RESTART. . . . . . . . . . . . . . . . . . .ON
   LINEAR PERTURBATION . . . . . . . . . . . . . .ON
   OFFSET TEMPERATURE FROM ABSOLUTE ZERO . . . . .  273.15    

 *** WARNING ***                         CP =       1.359   TIME= 11:09:09
 Material number 2 (used by element 373) should normally have at least   
 one MP or one TB type command associated with it.  Output of energy by  
 material may not be available.                                          

 *** NOTE ***                            CP =       1.359   TIME= 11:09:09
 The step data was checked and warning messages were found.              
  Please review output or errors file (                                  
 C:\Users\PAPERS~1\AppData\Local\Temp\ansys_etlukvhxzp\file.err ) for    
 these warning messages.                                                 

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:09  SEP 10, 2021 CP=      1.422

                                                                               

                      L O A D   S T E P   O P T I O N S

   SOLUTION TO BE PERTURBED CORRESPONDS TO
      TIME . . . . . . . . . . . . . . . . . . . .  1.0000    
      LOAD STEP. . . . . . . . . . . . . . . . . .     2
      SUBSTEP. . . . . . . . . . . . . . . . . . .     1
   STRESS-STIFFENING . . . . . . . . . . . . . . .    ON

 *** NOTE ***                            CP =       1.422   TIME= 11:09:09
 This SOLVE command is only used to generate the matrices needed to      
 perform the linear perturbation analysis.  The linear perturbation      
 analysis corresponds to time = 1 (load step = 2, substep = 1).  No      
 results are being written.                                              

 LINEAR PERTURBATION ANALYSIS PROCEDURE DELETES ALL
 BOUNDARY CONDITIONS EXCEPT CONSTRAINTS AND TEMPERATURES FROM DATABASE

 PARAMETER _THICKRATIO =     0.000000000    

 USE SYM. BLOCK LANCZOS MODE EXTRACTION METHOD
  EXTRACT   100 MODES
  NORMALIZE THE MODE SHAPES TO THE MASS MATRIX

 ERASE THE CURRENT DATABASE OUTPUT CONTROL TABLE.

 WRITE ALL  ITEMS TO THE DATABASE WITH A FREQUENCY OF NONE
   FOR ALL APPLICABLE ENTITIES

 WRITE NSOL ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 WRITE ETMP ITEMS TO THE DATABASE WITH A FREQUENCY OF ALL 
   FOR ALL APPLICABLE ENTITIES

 EXPAND ALL EXTRACTED MODES
  DO NOT CALCULATE ELEMENT RESULTS

 *GET  ANSINTER_  FROM  ACTI  ITEM=INT        VALUE=  0.00000000    

 *IF  ANSINTER_                         ( =   0.00000     )  NE  
      0                                 ( =   0.00000     )  THEN    

 *ENDIF

 *****  ANSYS SOLVE    COMMAND  *****

 *** NOTE ***                            CP =       1.531   TIME= 11:09:09
 There is no title defined for this analysis.                            

 *** SELECTION OF ELEMENT TECHNOLOGIES FOR APPLICABLE ELEMENTS ***
      --- GIVE SUGGESTIONS AND RESET THE KEY OPTIONS ---

 ELEMENT TYPE         1 IS SOLID186. KEYOPT(2) IS ALREADY SET AS SUGGESTED AND NO
 RESETTING IS NEEDED.

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:09  SEP 10, 2021 CP=      1.531

                                                                               

                       S O L U T I O N   O P T I O N S

   PROBLEM DIMENSIONALITY. . . . . . . . . . . . .3-D                  
   DEGREES OF FREEDOM. . . . . . UX   UY   UZ  
   ANALYSIS TYPE . . . . . . . . . . . . . . . . .MODAL                
      EXTRACTION METHOD. . . . . . . . . . . . . .BLOCK LANCZOS
   LINEAR PERTURBATION . . . . . . . . . . . . . .ON
   OFFSET TEMPERATURE FROM ABSOLUTE ZERO . . . . .  273.15    
   PRESTRESS EFFECTS INCLUDED IF AVAILABLE . . . .YES
   NUMBER OF MODES TO EXTRACT. . . . . . . . . . .   100
   GLOBALLY ASSEMBLED MATRIX . . . . . . . . . . .SYMMETRIC  
   NUMBER OF MODES TO EXPAND . . . . . . . . . . .ALL
   ELEMENT RESULTS CALCULATION . . . . . . . . . .OFF

 *** WARNING ***                         CP =       1.531   TIME= 11:09:09
 Material number 2 (used by element 373) should normally have at least   
 one MP or one TB type command associated with it.  Output of energy by  
 material may not be available.                                          

 *** NOTE ***                            CP =       1.531   TIME= 11:09:09
 The step data was checked and warning messages were found.              
  Please review output or errors file (                                  
 C:\Users\PAPERS~1\AppData\Local\Temp\ansys_etlukvhxzp\file.err ) for    
 these warning messages.                                                 

                      L O A D   S T E P   O P T I O N S

   LOAD STEP NUMBER. . . . . . . . . . . . . . . .     1
   THERMAL STRAINS INCLUDED IN THE LOAD VECTOR . .   YES
   PRINT OUTPUT CONTROLS . . . . . . . . . . . . .NO PRINTOUT
   DATABASE OUTPUT CONTROLS
      ITEM     FREQUENCY   COMPONENT
       ALL       NONE               
      NSOL        ALL               
      ETMP        ALL               

 *** WARNING ***                         CP =       1.594   TIME= 11:09:09
 The modal analysis has non-zero displacements defined, which will cause 
 a load vector to be generated.  The load vector may be used by the      
 mode superposition analyses.  This feature is not documented.           

                         ***********  PRECISE MASS SUMMARY  ***********

   TOTAL RIGID BODY MASS MATRIX ABOUT ORIGIN
               Translational mass               |   Coupled translational/rotational mass
         1178.2        0.0000        0.0000     |     0.0000        1413.9       -76.485    
         0.0000        1178.2        0.0000     |    -1413.9        0.0000        1.0669    
         0.0000        0.0000        1178.2     |     76.485       -1.0669        0.0000    
     ------------------------------------------ | ------------------------------------------
                                                |         Rotational mass (inertia)
                                                |     2268.3      -0.88451E-01   -1.2803    
                                                |   -0.88451E-01    2280.4       -91.782    
                                                |    -1.2803       -91.782        24.283    

   TOTAL MASS =  1178.2    
     The mass principal axes coincide with the global Cartesian axes

   CENTER OF MASS (X,Y,Z)=   0.90553E-03   0.64915E-01    1.2000    

   TOTAL INERTIA ABOUT CENTER OF MASS
         566.72      -0.19192E-01   0.44356E-13
       -0.19192E-01    583.70       0.13868E-11
        0.44356E-13   0.13868E-11    19.317    
     The inertia principal axes coincide with the global Cartesian axes

  *** MASS SUMMARY BY ELEMENT TYPE ***

  TYPE      MASS
     1   1178.23    

  BLOCK LANCZOS CALCULATION OF UP TO   100 EIGENVECTORS.
  NUMBER OF EQUATIONS              =         2402
  MAXIMUM WAVEFRONT                =          177
  MAXIMUM MODES STORED             =          100
  MINIMUM EIGENVALUE               =  0.00000E+00
  MAXIMUM EIGENVALUE               =  0.10000E+31

  Memory allocated for solver              =     6.907 MB
  Memory required for in-core solution     =     6.585 MB
  Memory required for out-of-core solution =     3.748 MB

 *** NOTE ***                            CP =       2.203   TIME= 11:09:09
 The Sparse Matrix Solver is currently running in the in-core memory     
 mode.  This memory mode uses the most amount of memory in order to      
 avoid using the hard drive as much as possible, which most often        
 results in the fastest solution time.  This mode is recommended if      
 enough physical memory is present to accommodate all of the solver      
 data.                                                                   

 *** WARNING ***                         CP =       8.641   TIME= 11:09:10
 1 Negative frequency found in the range [-100 : -10] Hz.  These         
 frequencies were not requested so they are not listed.  To extract      
 them, you can specify a negative shift (FREQB on MODOPT command).       
 Check your model carefully.                                             

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:10  SEP 10, 2021 CP=      8.641

                                                                               

 *** FREQUENCIES FROM BLOCK LANCZOS ITERATION ***

  MODE    FREQUENCY (HERTZ)      

    1     573.2415474366    
    2     607.6602931755    
    3     841.8417721182    
    4     869.9732240316    
    5     903.9746264978    
    6     909.4209154478    
    7     973.9627977415    
    8     1054.409034197    
    9     1163.253580573    
   10     1208.505801975    
   11     1293.741917990    
   12     1494.092478508    
   13     1583.462419600    
   14     1727.992387305    
   15     1801.909451148    
   16     1861.878166897    
   17     1899.562313107    
   18     1972.341284407    
   19     2229.883867080    
   20     2297.222797152    
   21     2332.388820910    
   22     2398.970277213    
   23     2587.418604226    
   24     2590.780975786    
   25     2603.413084599    
   26     2612.832526478    
   27     2633.606619284    
   28     2636.681343088    
   29     2697.773259265    
   30     2708.838311813    
   31     2739.748039959    
   32     2798.044286366    
   33     2824.736633389    
   34     2872.958018787    
   35     2874.926306322    
   36     2916.266150570    
   37     3006.318711218    
   38     3066.609002215    
   39     3197.695302914    
   40     3269.984199082    
   41     3326.720167194    
   42     3343.110512139    
   43     3392.484320380    
   44     3418.081493687    
   45     3597.732083843    
   46     3631.501830746    
   47     3645.559237860    
   48     3719.010539829    
   49     3777.355247823    
   50     3798.278543216    
   51     3846.779324844    
   52     3864.135144081    
   53     3871.485476623    
   54     3902.387827766    
   55     3906.765138654    
   56     4117.036102344    
   57     4135.427249878    
   58     4241.395831891    
   59     4320.309634151    
   60     4431.340806201    
   61     4492.874411224    
   62     4515.698292283    
   63     4534.646803680    
   64     4668.018851510    
   65     4757.326037584    
   66     4849.748292433    
   67     4977.680654488    
   68     5097.863106884    
   69     5120.830979286    
   70     5203.702759185    
   71     5255.307028242    
   72     5297.839219468    
   73     5337.333998776    
   74     5346.907965903    
   75     5359.219955226    
   76     5365.172094164    
   77     5374.000110049    
   78     5382.091812772    
   79     5400.375334804    
   80     5422.665434544    
   81     5465.445273425    
   82     5485.445298611    
   83     5516.426148125    
   84     5578.062322010    
   85     5588.389715488    
   86     5650.588251350    
   87     5699.516664744    
   88     5786.972051911    
   89     5834.326168673    
   90     5854.072357314    
   91     5885.728398830    
   92     6014.122363874    
   93     6093.251150843    
   94     6126.755722000    
   95     6214.316197491    
   96     6296.428174041    
   97     6320.073385477    
   98     6431.114210864    
   99     6448.743288021    
  100     6460.044353579    

 *** ANSYS - ENGINEERING ANALYSIS SYSTEM  RELEASE 2021 R2          21.2     ***
 Ansys Mechanical Enterprise Academic Student      
 00000000  VERSION=WINDOWS x64   11:09:10  SEP 10, 2021 CP=      8.891

                                                                               

          ***** PARTICIPATION FACTOR CALCULATION *****  X  DIRECTION
                                                                                  CUMULATIVE     RATIO EFF.MASS
  MODE   FREQUENCY       PERIOD      PARTIC.FACTOR     RATIO    EFFECTIVE MASS   MASS FRACTION   TO TOTAL MASS
     1     573.242       0.17445E-02    10.925        1.000000     119.353        0.677731        0.101298    
     2     607.660       0.16457E-02    1.1484        0.105116     1.31879        0.685219        0.111929E-02
     3     841.842       0.11879E-02  -0.37847E-01    0.003464    0.143241E-02    0.685227        0.121572E-05
     4     869.973       0.11495E-02   0.74448E-01    0.006815    0.554247E-02    0.685259        0.470404E-05
     5     903.975       0.11062E-02   0.37926E-01    0.003472    0.143836E-02    0.685267        0.122078E-05
     6     909.421       0.10996E-02   0.30260E-01    0.002770    0.915686E-03    0.685272        0.777167E-06
     7     973.963       0.10267E-02  -0.21603E-01    0.001977    0.466695E-03    0.685275        0.396096E-06
     8     1054.41       0.94840E-03   0.52116E-01    0.004770    0.271611E-02    0.685290        0.230524E-05
     9     1163.25       0.85966E-03   0.23702        0.021696    0.561794E-01    0.685609        0.476810E-04
    10     1208.51       0.82747E-03    4.5440        0.415930     20.6478        0.802855        0.175243E-01
    11     1293.74       0.77295E-03  -0.48938        0.044795    0.239497        0.804215        0.203267E-03
    12     1494.09       0.66930E-03  -0.12009        0.010993    0.144228E-01    0.804297        0.122410E-04
    13     1583.46       0.63153E-03   0.11059        0.010123    0.122297E-01    0.804366        0.103797E-04
    14     1727.99       0.57871E-03   0.20869        0.019102    0.435517E-01    0.804614        0.369635E-04
    15     1801.91       0.55497E-03   0.23717E-01    0.002171    0.562510E-03    0.804617        0.477417E-06
    16     1861.88       0.53709E-03  -0.17965        0.016444    0.322748E-01    0.804800        0.273925E-04
    17     1899.56       0.52644E-03   -1.6971        0.155347     2.88032        0.821156        0.244460E-02
    18     1972.34       0.50701E-03  -0.28466        0.026056    0.810332E-01    0.821616        0.687751E-04
    19     2229.88       0.44845E-03  -0.15585E-01    0.001427    0.242897E-03    0.821617        0.206153E-06
    20     2297.22       0.43531E-03    2.2009        0.201456     4.84389        0.849123        0.411114E-02
    21     2332.39       0.42874E-03   0.82648        0.075651    0.683062        0.853001        0.579734E-03
    22     2398.97       0.41685E-03   0.13404        0.012269    0.179667E-01    0.853103        0.152488E-04
    23     2587.42       0.38649E-03  -0.15559        0.014241    0.242072E-01    0.853241        0.205453E-04
    24     2590.78       0.38598E-03  -0.20843E-01    0.001908    0.434442E-03    0.853243        0.368723E-06
    25     2603.41       0.38411E-03   0.85530E-01    0.007829    0.731536E-02    0.853285        0.620875E-05
    26     2612.83       0.38273E-03  -0.43590        0.039900    0.190009        0.854364        0.161266E-03
    27     2633.61       0.37971E-03  -0.15634        0.014311    0.244426E-01    0.854502        0.207451E-04
    28     2636.68       0.37926E-03   0.10458        0.009573    0.109370E-01    0.854565        0.928250E-05
    29     2697.77       0.37068E-03   0.12228        0.011193    0.149528E-01    0.854649        0.126909E-04
    30     2708.84       0.36916E-03  -0.72722        0.066566    0.528854        0.857652        0.448852E-03
    31     2739.75       0.36500E-03   0.22666        0.020747    0.513728E-01    0.857944        0.436015E-04
    32     2798.04       0.35739E-03   0.76265E-01    0.006981    0.581639E-02    0.857977        0.493653E-05
    33     2824.74       0.35402E-03   0.87101        0.079727    0.758662        0.862285        0.643898E-03
    34     2872.96       0.34807E-03  -0.15948        0.014598    0.254336E-01    0.862430        0.215862E-04
    35     2874.93       0.34784E-03  -0.19204        0.017578    0.368788E-01    0.862639        0.313000E-04
    36     2916.27       0.34290E-03  -0.65304        0.059775    0.426460        0.865061        0.361948E-03
    37     3006.32       0.33263E-03   0.75321E-01    0.006894    0.567323E-02    0.865093        0.481502E-05
    38     3066.61       0.32609E-03   0.74889        0.068549    0.560840        0.868277        0.476000E-03
    39     3197.70       0.31273E-03    1.8957        0.173522     3.59372        0.888684        0.305009E-02
    40     3269.98       0.30581E-03    1.7345        0.158768     3.00856        0.905768        0.255345E-02
    41     3326.72       0.30060E-03   0.97324        0.089085    0.947200        0.911146        0.803914E-03
    42     3343.11       0.29912E-03  -0.29099        0.026636    0.846766E-01    0.911627        0.718674E-04
    43     3392.48       0.29477E-03   0.77085        0.070559    0.594208        0.915001        0.504320E-03
    44     3418.08       0.29256E-03   0.48958        0.044813    0.239691        0.916362        0.203432E-03
    45     3597.73       0.27795E-03    1.4570        0.133368     2.12293        0.928417        0.180179E-02
    46     3631.50       0.27537E-03  -0.73571E-01    0.006734    0.541268E-02    0.928448        0.459389E-05
    47     3645.56       0.27431E-03   -1.2818        0.117329     1.64302        0.937777        0.139448E-02
    48     3719.01       0.26889E-03   0.82888        0.075871    0.687038        0.941679        0.583108E-03
    49     3777.36       0.26474E-03   0.32130        0.029410    0.103231        0.942265        0.876152E-04
    50     3798.28       0.26328E-03   0.31101        0.028468    0.967277E-01    0.942814        0.820954E-04
    51     3846.78       0.25996E-03   0.27212        0.024908    0.740499E-01    0.943235        0.628482E-04
    52     3864.14       0.25879E-03  -0.30728        0.028127    0.944210E-01    0.943771        0.801377E-04
    53     3871.49       0.25830E-03  -0.76638E-01    0.007015    0.587343E-02    0.943804        0.498494E-05
    54     3902.39       0.25625E-03  -0.19361        0.017722    0.374848E-01    0.944017        0.318144E-04
    55     3906.77       0.25597E-03  -0.15132        0.013850    0.228962E-01    0.944147        0.194327E-04
    56     4117.04       0.24289E-03   0.33792        0.030931    0.114189        0.944795        0.969153E-04
    57     4135.43       0.24181E-03  -0.51380        0.047030    0.263991        0.946294        0.224056E-03
    58     4241.40       0.23577E-03   0.73551E-01    0.006732    0.540978E-02    0.946325        0.459142E-05
    59     4320.31       0.23146E-03   -1.6573        0.151696     2.74650        0.961921        0.233103E-02
    60     4431.34       0.22567E-03   0.43466        0.039787    0.188933        0.962994        0.160352E-03
    61     4492.87       0.22257E-03   0.10247        0.009379    0.104995E-01    0.963053        0.891125E-05
    62     4515.70       0.22145E-03  -0.17651        0.016156    0.311544E-01    0.963230        0.264416E-04
    63     4534.65       0.22052E-03   0.43246        0.039585    0.187019        0.964292        0.158728E-03
    64     4668.02       0.21422E-03  -0.25766E-01    0.002358    0.663891E-03    0.964296        0.563462E-06
    65     4757.33       0.21020E-03  -0.92804E-01    0.008495    0.861256E-02    0.964345        0.730971E-05
    66     4849.75       0.20620E-03   0.11764        0.010768    0.138384E-01    0.964423        0.117450E-04
    67     4977.68       0.20090E-03    1.5086        0.138091     2.27595        0.977347        0.193166E-02
    68     5097.86       0.19616E-03   0.30674        0.028077    0.940893E-01    0.977881        0.798562E-04
    69     5120.83       0.19528E-03  -0.38878        0.035586    0.151147        0.978740        0.128282E-03
    70     5203.70       0.19217E-03  -0.13270        0.012147    0.176093E-01    0.978840        0.149455E-04
    71     5255.31       0.19028E-03  -0.10339        0.009464    0.106901E-01    0.978900        0.907302E-05
    72     5297.84       0.18876E-03   0.30407E-01    0.002783    0.924602E-03    0.978905        0.784735E-06
    73     5337.33       0.18736E-03  -0.42679E-01    0.003907    0.182147E-02    0.978916        0.154593E-05
    74     5346.91       0.18702E-03   0.30405E-01    0.002783    0.924475E-03    0.978921        0.784628E-06
    75     5359.22       0.18659E-03   0.27561E-03    0.000025    0.759583E-07    0.978921        0.644679E-10
    76     5365.17       0.18639E-03   0.81811E-02    0.000749    0.669302E-04    0.978921        0.568055E-07
    77     5374.00       0.18608E-03  -0.69687E-02    0.000638    0.485630E-04    0.978922        0.412167E-07
    78     5382.09       0.18580E-03  -0.85789E-02    0.000785    0.735973E-04    0.978922        0.624640E-07
    79     5400.38       0.18517E-03   0.47541E-01    0.004352    0.226017E-02    0.978935        0.191827E-05
    80     5422.67       0.18441E-03   0.64894E-01    0.005940    0.421128E-02    0.978959        0.357423E-05
    81     5465.45       0.18297E-03  -0.26765        0.024499    0.716374E-01    0.979366        0.608006E-04
    82     5485.45       0.18230E-03  -0.47564        0.043537    0.226232        0.980650        0.192009E-03
    83     5516.43       0.18128E-03  -0.54100E-02    0.000495    0.292683E-04    0.980650        0.248408E-07
    84     5578.06       0.17927E-03   0.38187E-01    0.003495    0.145823E-02    0.980659        0.123764E-05
    85     5588.39       0.17894E-03  -0.11664        0.010677    0.136053E-01    0.980736        0.115472E-04
    86     5650.59       0.17697E-03   -1.1963        0.109503     1.43115        0.988863        0.121466E-02
    87     5699.52       0.17545E-03  -0.39814        0.036444    0.158519        0.989763        0.134539E-03
    88     5786.97       0.17280E-03  -0.33073        0.030273    0.109383        0.990384        0.928366E-04
    89     5834.33       0.17140E-03   0.70370E-01    0.006441    0.495192E-02    0.990412        0.420283E-05
    90     5854.07       0.17082E-03   0.13142        0.012029    0.172701E-01    0.990510        0.146576E-04
    91     5885.73       0.16990E-03   0.29443        0.026950    0.866871E-01    0.991002        0.735737E-04
    92     6014.12       0.16628E-03   0.50555E-01    0.004627    0.255579E-02    0.991017        0.216917E-05
    93     6093.25       0.16412E-03  -0.45540E-02    0.000417    0.207387E-04    0.991017        0.176015E-07
    94     6126.76       0.16322E-03  -0.10483        0.009595    0.109891E-01    0.991079        0.932674E-05
    95     6214.32       0.16092E-03   0.96988E-01    0.008878    0.940663E-02    0.991133        0.798366E-05
    96     6296.43       0.15882E-03   0.29545        0.027044    0.872891E-01    0.991628        0.740847E-04
    97     6320.07       0.15823E-03    1.1594        0.106123     1.34416        0.999261        0.114082E-02
    98     6431.11       0.15549E-03   0.34773        0.031829    0.120915        0.999948        0.102624E-03
    99     6448.74       0.15507E-03  -0.39044E-01    0.003574    0.152441E-02    0.999956        0.129381E-05
   100     6460.04       0.15480E-03   0.87772E-01    0.008034    0.770391E-02     1.00000        0.653852E-05
 -----------------------------------------------------------------------------------------------------------------
   sum                                                             176.107                        0.149467    
 -----------------------------------------------------------------------------------------------------------------

          ***** PARTICIPATION FACTOR CALCULATION *****  Y  DIRECTION
                                                                                  CUMULATIVE     RATIO EFF.MASS
  MODE   FREQUENCY       PERIOD      PARTIC.FACTOR     RATIO    EFFECTIVE MASS   MASS FRACTION   TO TOTAL MASS
     1     573.242       0.17445E-02   0.15878        0.032009    0.252102E-01    0.178528E-03    0.213966E-04
     2     607.660       0.16457E-02   0.41112        0.082880    0.169016        0.137542E-02    0.143448E-03
     3     841.842       0.11879E-02    4.2778        0.862394     18.2994        0.130964        0.155312E-01
     4     869.973       0.11495E-02    2.0341        0.410070     4.13755        0.160264        0.351166E-02
     5     903.975       0.11062E-02    1.8423        0.371409     3.39416        0.184300        0.288071E-02
     6     909.421       0.10996E-02    1.2753        0.257095     1.62635        0.195817        0.138033E-02
     7     973.963       0.10267E-02  -0.52660        0.106161    0.277306        0.197781        0.235357E-03
     8     1054.41       0.94840E-03  -0.38598        0.077812    0.148978        0.198836        0.126441E-03
     9     1163.25       0.85966E-03  -0.24819        0.050034    0.615979E-01    0.199272        0.522798E-04
    10     1208.51       0.82747E-03  -0.84641        0.170635    0.716415        0.204346        0.608041E-03
    11     1293.74       0.77295E-03   -2.8417        0.572885     8.07537        0.261532        0.685378E-02
    12     1494.09       0.66930E-03   -1.9872        0.400609     3.94883        0.289496        0.335148E-02
    13     1583.46       0.63153E-03    3.5903        0.723803     12.8904        0.380780        0.109405E-01
    14     1727.99       0.57871E-03    3.9772        0.801804     15.8184        0.492799        0.134255E-01
    15     1801.91       0.55497E-03   0.37476        0.075551    0.140446        0.493794        0.119201E-03
    16     1861.88       0.53709E-03   0.66932        0.134934    0.447992        0.496966        0.380223E-03
    17     1899.56       0.52644E-03   0.19412        0.039134    0.376819E-01    0.497233        0.319816E-04
    18     1972.34       0.50701E-03    1.0440        0.210469     1.08994        0.504951        0.925063E-03
    19     2229.88       0.44845E-03    2.5192        0.507875     6.34660        0.549895        0.538654E-02
    20     2297.22       0.43531E-03   0.47158        0.095069    0.222386        0.551470        0.188745E-03
    21     2332.39       0.42874E-03   -1.0180        0.205227     1.03632        0.558809        0.879556E-03
    22     2398.97       0.41685E-03    4.9604        1.000000     24.6052        0.733052        0.208831E-01
    23     2587.42       0.38649E-03  -0.47961E-01    0.009669    0.230025E-02    0.733068        0.195228E-05
    24     2590.78       0.38598E-03   0.15756E-01    0.003176    0.248239E-03    0.733070        0.210687E-06
    25     2603.41       0.38411E-03   -1.7161        0.345957     2.94491        0.753924        0.249943E-02
    26     2612.83       0.38273E-03  -0.85751E-01    0.017287    0.735322E-02    0.753977        0.624088E-05
    27     2633.61       0.37971E-03   0.35111        0.070782    0.123276        0.754850        0.104628E-03
    28     2636.68       0.37926E-03   -1.5580        0.314097     2.42747        0.772040        0.206026E-02
    29     2697.77       0.37068E-03  -0.71479        0.144099    0.510919        0.775658        0.433631E-03
    30     2708.84       0.36916E-03   0.15045        0.030330    0.226353E-01    0.775818        0.192112E-04
    31     2739.75       0.36500E-03  -0.16667        0.033601    0.277802E-01    0.776015        0.235778E-04
    32     2798.04       0.35739E-03   0.40619        0.081887    0.164990        0.777183        0.140032E-03
    33     2824.74       0.35402E-03  -0.15946E-01    0.003215    0.254274E-03    0.777185        0.215809E-06
    34     2872.96       0.34807E-03   0.72323E-02    0.001458    0.523064E-04    0.777185        0.443939E-07
    35     2874.93       0.34784E-03   0.24724E-02    0.000498    0.611257E-05    0.777186        0.518791E-08
    36     2916.27       0.34290E-03   0.23658E-01    0.004769    0.559692E-03    0.777190        0.475026E-06
    37     3006.32       0.33263E-03   -1.0492        0.211522     1.10087        0.784985        0.934342E-03
    38     3066.61       0.32609E-03  -0.53473E-02    0.001078    0.285938E-04    0.784986        0.242684E-07
    39     3197.70       0.31273E-03  -0.16133        0.032524    0.260269E-01    0.785170        0.220898E-04
    40     3269.98       0.30581E-03  -0.35107        0.070775    0.123248        0.786043        0.104604E-03
    41     3326.72       0.30060E-03  -0.49216        0.099218    0.242220        0.787758        0.205578E-03
    42     3343.11       0.29912E-03   0.98080        0.197727    0.961965        0.794570        0.816446E-03
    43     3392.48       0.29477E-03    2.8542        0.575404     8.14653        0.852260        0.691418E-02
    44     3418.08       0.29256E-03  -0.29354        0.059178    0.861680E-01    0.852870        0.731332E-04
    45     3597.73       0.27795E-03  -0.94481E-01    0.019047    0.892675E-02    0.852934        0.757637E-05
    46     3631.50       0.27537E-03   0.67047        0.135166    0.449535        0.856117        0.381533E-03
    47     3645.56       0.27431E-03   0.60417E-02    0.001218    0.365017E-04    0.856117        0.309799E-07
    48     3719.01       0.26889E-03  -0.10286        0.020736    0.105794E-01    0.856192        0.897900E-05
    49     3777.36       0.26474E-03   0.48040        0.096848    0.230784        0.857827        0.195873E-03
    50     3798.28       0.26328E-03  -0.43638        0.087974    0.190431        0.859175        0.161624E-03
    51     3846.78       0.25996E-03  -0.19973E-01    0.004026    0.398903E-03    0.859178        0.338560E-06
    52     3864.14       0.25879E-03   0.71000E-01    0.014314    0.504104E-02    0.859214        0.427847E-05
    53     3871.49       0.25830E-03  -0.39440        0.079510    0.155552        0.860315        0.132021E-03
    54     3902.39       0.25625E-03   0.48641E-01    0.009806    0.236599E-02    0.860332        0.200808E-05
    55     3906.77       0.25597E-03  -0.24762        0.049920    0.613152E-01    0.860766        0.520399E-04
    56     4117.04       0.24289E-03  -0.60586E-01    0.012214    0.367065E-02    0.860792        0.311538E-05
    57     4135.43       0.24181E-03   0.38649E-01    0.007792    0.149376E-02    0.860803        0.126780E-05
    58     4241.40       0.23577E-03   0.14361        0.028951    0.206229E-01    0.860949        0.175032E-04
    59     4320.31       0.23146E-03   0.49539        0.099871    0.245416        0.862687        0.208291E-03
    60     4431.34       0.22567E-03  -0.87085E-01    0.017556    0.758377E-02    0.862740        0.643655E-05
    61     4492.87       0.22257E-03   0.63896        0.128813    0.408269        0.865632        0.346509E-03
    62     4515.70       0.22145E-03   -1.3749        0.277184     1.89045        0.879019        0.160447E-02
    63     4534.65       0.22052E-03    1.6837        0.339437     2.83495        0.899095        0.240610E-02
    64     4668.02       0.21422E-03  -0.19170        0.038646    0.367486E-01    0.899355        0.311896E-04
    65     4757.33       0.21020E-03   0.65987E-01    0.013303    0.435423E-02    0.899386        0.369555E-05
    66     4849.75       0.20620E-03    1.3583        0.273828     1.84495        0.912451        0.156586E-02
    67     4977.68       0.20090E-03  -0.56396        0.113692    0.318045        0.914703        0.269934E-03
    68     5097.86       0.19616E-03   0.82000        0.165311    0.672406        0.919465        0.570689E-03
    69     5120.83       0.19528E-03   -1.2003        0.241974     1.44067        0.929667        0.122274E-02
    70     5203.70       0.19217E-03  -0.94777E-01    0.019107    0.898271E-02    0.929731        0.762387E-05
    71     5255.31       0.19028E-03    1.8981        0.382647     3.60266        0.955243        0.305767E-02
    72     5297.84       0.18876E-03   0.15558        0.031364    0.242039E-01    0.955414        0.205425E-04
    73     5337.33       0.18736E-03   0.64006        0.129034    0.409671        0.958316        0.347699E-03
    74     5346.91       0.18702E-03  -0.24347        0.049083    0.592769E-01    0.958735        0.503099E-04
    75     5359.22       0.18659E-03   0.32291E-01    0.006510    0.104273E-02    0.958743        0.884992E-06
    76     5365.17       0.18639E-03  -0.66111E-01    0.013328    0.437066E-02    0.958774        0.370950E-05
    77     5374.00       0.18608E-03   0.14500        0.029232    0.210250E-01    0.958923        0.178445E-04
    78     5382.09       0.18580E-03   0.94552E-01    0.019061    0.894004E-02    0.958986        0.758766E-05
    79     5400.38       0.18517E-03  -0.73608        0.148392    0.541813        0.962823        0.459852E-03
    80     5422.67       0.18441E-03  -0.89196        0.179817    0.795587        0.968457        0.675236E-03
    81     5465.45       0.18297E-03   0.76633        0.154491    0.587266        0.972616        0.498428E-03
    82     5485.45       0.18230E-03  -0.25090        0.050581    0.629515E-01    0.973061        0.534287E-04
    83     5516.43       0.18128E-03  -0.53738E-01    0.010833    0.288772E-02    0.973082        0.245089E-05
    84     5578.06       0.17927E-03  -0.85721E-01    0.017281    0.734801E-02    0.973134        0.623646E-05
    85     5588.39       0.17894E-03  -0.69697E-01    0.014051    0.485774E-02    0.973168        0.412289E-05
    86     5650.59       0.17697E-03   0.32629        0.065780    0.106466        0.973922        0.903609E-04
    87     5699.52       0.17545E-03  -0.73851        0.148882    0.545399        0.977784        0.462895E-03
    88     5786.97       0.17280E-03  -0.74203        0.149592    0.550610        0.981684        0.467318E-03
    89     5834.33       0.17140E-03   0.12815        0.025835    0.164233E-01    0.981800        0.139389E-04
    90     5854.07       0.17082E-03   0.77231E-01    0.015570    0.596463E-02    0.981842        0.506234E-05
    91     5885.73       0.16990E-03  -0.65618E-02    0.001323    0.430571E-04    0.981842        0.365438E-07
    92     6014.12       0.16628E-03  -0.15253        0.030750    0.232664E-01    0.982007        0.197468E-04
    93     6093.25       0.16412E-03   0.16218        0.032695    0.263018E-01    0.982193        0.223231E-04
    94     6126.76       0.16322E-03  -0.92412        0.186302    0.854004        0.988241        0.724817E-03
    95     6214.32       0.16092E-03   0.98586        0.198749    0.971930        0.995124        0.824903E-03
    96     6296.43       0.15882E-03  -0.13357        0.026927    0.178403E-01    0.995250        0.151416E-04
    97     6320.07       0.15823E-03  -0.34422        0.069395    0.118489        0.996089        0.100565E-03
    98     6431.11       0.15549E-03   0.57732        0.116386    0.333298        0.998450        0.282879E-03
    99     6448.74       0.15507E-03  -0.39810        0.080256    0.158484        0.999572        0.134510E-03
   100     6460.04       0.15480E-03   0.24586        0.049566    0.604489E-01     1.00000        0.513047E-04
 -----------------------------------------------------------------------------------------------------------------
   sum                                                             141.212                        0.119850    
 -----------------------------------------------------------------------------------------------------------------

          ***** PARTICIPATION FACTOR CALCULATION *****  Z  DIRECTION
                                                                                  CUMULATIVE     RATIO EFF.MASS
  MODE   FREQUENCY       PERIOD      PARTIC.FACTOR     RATIO    EFFECTIVE MASS   MASS FRACTION   TO TOTAL MASS
     1     573.242       0.17445E-02   0.51034E-01    0.002200    0.260452E-02    0.234481E-05    0.221053E-05
     2     607.660       0.16457E-02  -0.43714        0.018844    0.191087        0.174378E-03    0.162181E-03
     3     841.842       0.11879E-02  -0.25721        0.011087    0.661559E-01    0.233937E-03    0.561483E-04
     4     869.973       0.11495E-02    2.7226        0.117362     7.41249        0.690728E-02    0.629118E-02
     5     903.975       0.11062E-02   -20.054        0.864481     402.177        0.368981        0.341339    
     6     909.421       0.10996E-02    23.198        1.000000     538.154        0.853472        0.456746    
     7     973.963       0.10267E-02  -0.89153        0.038431    0.794833        0.854188        0.674596E-03
     8     1054.41       0.94840E-03   -1.0625        0.045802     1.12896        0.855204        0.958177E-03
     9     1163.25       0.85966E-03   0.16305        0.007029    0.265850E-01    0.855228        0.225634E-04
    10     1208.51       0.82747E-03  -0.28450E-01    0.001226    0.809376E-03    0.855229        0.686939E-06
    11     1293.74       0.77295E-03  -0.66873E-04    0.000003    0.447195E-08    0.855229        0.379546E-11
    12     1494.09       0.66930E-03   0.13992E-01    0.000603    0.195765E-03    0.855229        0.166151E-06
    13     1583.46       0.63153E-03   0.49676E-01    0.002141    0.246774E-02    0.855231        0.209444E-05
    14     1727.99       0.57871E-03   0.99217E-01    0.004277    0.984398E-02    0.855240        0.835486E-05
    15     1801.91       0.55497E-03   0.21416E-01    0.000923    0.458658E-03    0.855240        0.389275E-06
    16     1861.88       0.53709E-03   0.14065        0.006063    0.197830E-01    0.855258        0.167904E-04
    17     1899.56       0.52644E-03  -0.22189E-01    0.000956    0.492337E-03    0.855258        0.417860E-06
    18     1972.34       0.50701E-03   0.77957E-01    0.003360    0.607725E-02    0.855264        0.515793E-05
    19     2229.88       0.44845E-03   0.45369        0.019557    0.205837        0.855449        0.174700E-03
    20     2297.22       0.43531E-03  -0.21878        0.009431    0.478626E-01    0.855492        0.406223E-04
    21     2332.39       0.42874E-03   0.53968        0.023264    0.291260        0.855755        0.247200E-03
    22     2398.97       0.41685E-03   0.47383E-01    0.002043    0.224510E-02    0.855757        0.190548E-05
    23     2587.42       0.38649E-03  -0.64890        0.027972    0.421070        0.856136        0.357374E-03
    24     2590.78       0.38598E-03   0.21302E-02    0.000092    0.453768E-05    0.856136        0.385126E-08
    25     2603.41       0.38411E-03   -4.0785        0.175811     16.6341        0.871111        0.141178E-01
    26     2612.83       0.38273E-03  -0.24541        0.010579    0.602280E-01    0.871165        0.511171E-04
    27     2633.61       0.37971E-03  -0.27487        0.011849    0.755517E-01    0.871233        0.641228E-04
    28     2636.68       0.37926E-03    7.4617        0.321653     55.6776        0.921359        0.472551E-01
    29     2697.77       0.37068E-03   -3.9765        0.171415     15.8127        0.935595        0.134207E-01
    30     2708.84       0.36916E-03   0.27746        0.011960    0.769825E-01    0.935664        0.653371E-04
    31     2739.75       0.36500E-03  -0.49628        0.021393    0.246295        0.935886        0.209037E-03
    32     2798.04       0.35739E-03   0.90681        0.039090    0.822302        0.936626        0.697910E-03
    33     2824.74       0.35402E-03  -0.64379E-01    0.002775    0.414471E-02    0.936630        0.351773E-05
    34     2872.96       0.34807E-03   0.44174        0.019042    0.195133        0.936806        0.165614E-03
    35     2874.93       0.34784E-03  -0.10218        0.004405    0.104405E-01    0.936815        0.886114E-05
    36     2916.27       0.34290E-03  -0.28981E-01    0.001249    0.839892E-03    0.936816        0.712840E-06
    37     3006.32       0.33263E-03   0.66015        0.028457    0.435800        0.937208        0.369876E-03
    38     3066.61       0.32609E-03   0.54626E-01    0.002355    0.298397E-02    0.937211        0.253258E-05
    39     3197.70       0.31273E-03   0.70871E-01    0.003055    0.502271E-02    0.937215        0.426291E-05
    40     3269.98       0.30581E-03   0.22363        0.009640    0.500104E-01    0.937260        0.424452E-04
    41     3326.72       0.30060E-03   0.82149        0.035412    0.674840        0.937868        0.572755E-03
    42     3343.11       0.29912E-03    3.7558        0.161902     14.1062        0.950567        0.119723E-01
    43     3392.48       0.29477E-03  -0.45764E-01    0.001973    0.209430E-02    0.950569        0.177749E-05
    44     3418.08       0.29256E-03  -0.53656E-01    0.002313    0.287901E-02    0.950572        0.244349E-05
    45     3597.73       0.27795E-03   0.74311E-01    0.003203    0.552207E-02    0.950577        0.468673E-05
    46     3631.50       0.27537E-03   -2.2273        0.096011     4.96073        0.955043        0.421031E-02
    47     3645.56       0.27431E-03   0.32843        0.014158    0.107868        0.955140        0.915509E-04
    48     3719.01       0.26889E-03  -0.13811        0.005954    0.190750E-01    0.955157        0.161894E-04
    49     3777.36       0.26474E-03  -0.24339        0.010492    0.592390E-01    0.955211        0.502777E-04
    50     3798.28       0.26328E-03  -0.16732        0.007213    0.279958E-01    0.955236        0.237608E-04
    51     3846.78       0.25996E-03   0.46222        0.019925    0.213648        0.955428        0.181329E-03
    52     3864.14       0.25879E-03  -0.19346        0.008339    0.374250E-01    0.955462        0.317636E-04
    53     3871.49       0.25830E-03   0.11248        0.004849    0.126512E-01    0.955473        0.107374E-04
    54     3902.39       0.25625E-03  -0.37814E-01    0.001630    0.142989E-02    0.955474        0.121358E-05
    55     3906.77       0.25597E-03   0.84811E-01    0.003656    0.719295E-02    0.955481        0.610486E-05
    56     4117.04       0.24289E-03   0.50942        0.021960    0.259508        0.955715        0.220252E-03
    57     4135.43       0.24181E-03   0.59917E-01    0.002583    0.359007E-02    0.955718        0.304699E-05
    58     4241.40       0.23577E-03   0.20360        0.008776    0.414510E-01    0.955755        0.351806E-04
    59     4320.31       0.23146E-03   0.19042E-01    0.000821    0.362579E-03    0.955755        0.307731E-06
    60     4431.34       0.22567E-03   0.15948E-01    0.000687    0.254350E-03    0.955756        0.215874E-06
    61     4492.87       0.22257E-03  -0.35327E-01    0.001523    0.124801E-02    0.955757        0.105922E-05
    62     4515.70       0.22145E-03   0.45936E-01    0.001980    0.211008E-02    0.955759        0.179088E-05
    63     4534.65       0.22052E-03  -0.77134E-01    0.003325    0.594960E-02    0.955764        0.504958E-05
    64     4668.02       0.21422E-03   -5.8381        0.251665     34.0840        0.986449        0.289280E-01
    65     4757.33       0.21020E-03  -0.69530E-01    0.002997    0.483442E-02    0.986454        0.410310E-05
    66     4849.75       0.20620E-03  -0.88163        0.038004    0.777272        0.987153        0.659692E-03
    67     4977.68       0.20090E-03  -0.11056        0.004766    0.122237E-01    0.987164        0.103746E-04
    68     5097.86       0.19616E-03   0.18304        0.007890    0.335038E-01    0.987195        0.284356E-04
    69     5120.83       0.19528E-03  -0.27313        0.011774    0.745996E-01    0.987262        0.633147E-04
    70     5203.70       0.19217E-03  -0.47232E-01    0.002036    0.223086E-02    0.987264        0.189339E-05
    71     5255.31       0.19028E-03  -0.24175        0.010421    0.584417E-01    0.987316        0.496010E-04
    72     5297.84       0.18876E-03  -0.19525E-01    0.000842    0.381236E-03    0.987317        0.323565E-06
    73     5337.33       0.18736E-03   0.31888        0.013746    0.101684        0.987408        0.863018E-04
    74     5346.91       0.18702E-03  -0.19660        0.008475    0.386532E-01    0.987443        0.328061E-04
    75     5359.22       0.18659E-03   0.43337        0.018681    0.187806        0.987612        0.159396E-03
    76     5365.17       0.18639E-03  -0.14447        0.006228    0.208724E-01    0.987631        0.177150E-04
    77     5374.00       0.18608E-03  -0.15824        0.006821    0.250404E-01    0.987654        0.212525E-04
    78     5382.09       0.18580E-03   0.52265E-01    0.002253    0.273168E-02    0.987656        0.231845E-05
    79     5400.38       0.18517E-03   0.52549E-01    0.002265    0.276145E-02    0.987658        0.234372E-05
    80     5422.67       0.18441E-03   0.22865E-01    0.000986    0.522796E-03    0.987659        0.443712E-06
    81     5465.45       0.18297E-03   0.11444        0.004933    0.130956E-01    0.987671        0.111146E-04
    82     5485.45       0.18230E-03  -0.19229E-01    0.000829    0.369743E-03    0.987671        0.313811E-06
    83     5516.43       0.18128E-03   0.11891        0.005126    0.141401E-01    0.987684        0.120011E-04
    84     5578.06       0.17927E-03  -0.26764E-01    0.001154    0.716320E-03    0.987684        0.607960E-06
    85     5588.39       0.17894E-03   0.73252E-01    0.003158    0.536592E-02    0.987689        0.455421E-05
    86     5650.59       0.17697E-03  -0.82348E-02    0.000355    0.678119E-04    0.987689        0.575538E-07
    87     5699.52       0.17545E-03   0.13111E-01    0.000565    0.171897E-03    0.987689        0.145894E-06
    88     5786.97       0.17280E-03  -0.26780E-01    0.001154    0.717153E-03    0.987690        0.608668E-06
    89     5834.33       0.17140E-03  -0.26813E-01    0.001156    0.718910E-03    0.987691        0.610159E-06
    90     5854.07       0.17082E-03  -0.52437E-03    0.000023    0.274964E-06    0.987691        0.233369E-09
    91     5885.73       0.16990E-03   0.57781E-03    0.000025    0.333864E-06    0.987691        0.283359E-09
    92     6014.12       0.16628E-03  -0.44850E-01    0.001933    0.201154E-02    0.987693        0.170725E-05
    93     6093.25       0.16412E-03   0.18530E-01    0.000799    0.343367E-03    0.987693        0.291425E-06
    94     6126.76       0.16322E-03  -0.13668        0.005892    0.186821E-01    0.987710        0.158560E-04
    95     6214.32       0.16092E-03  -0.10056        0.004335    0.101131E-01    0.987719        0.858325E-05
    96     6296.43       0.15882E-03  -0.18599E-01    0.000802    0.345930E-03    0.987719        0.293600E-06
    97     6320.07       0.15823E-03  -0.49522E-01    0.002135    0.245242E-02    0.987721        0.208144E-05
    98     6431.11       0.15549E-03   0.81149        0.034981    0.658513        0.988314        0.558898E-03
    99     6448.74       0.15507E-03    3.5097        0.151293     12.3181        0.999404        0.104547E-01
   100     6460.04       0.15480E-03   0.81369        0.035076    0.662086         1.00000        0.561931E-03
 -----------------------------------------------------------------------------------------------------------------
   sum                                                             1110.76                        0.942733    
 -----------------------------------------------------------------------------------------------------------------

          ***** PARTICIPATION FACTOR CALCULATION *****ROTX DIRECTION
                                                                                  CUMULATIVE     RATIO EFF.MASS
  MODE   FREQUENCY       PERIOD      PARTIC.FACTOR     RATIO    EFFECTIVE MASS   MASS FRACTION   TO TOTAL MASS
     1     573.242       0.17445E-02   0.23277        0.035760    0.541830E-01    0.161974E-03    0.238866E-04
     2     607.660       0.16457E-02   -5.2936        0.813236     28.0222        0.839311E-01    0.123536E-01
     3     841.842       0.11879E-02   -6.5093        1.000000     42.3711        0.210595        0.186793E-01
     4     869.973       0.11495E-02   -4.2950        0.659826     18.4471        0.265740        0.813241E-02
     5     903.975       0.11062E-02  -0.49954        0.076743    0.249545        0.266486        0.110012E-03
     6     909.421       0.10996E-02    2.6208        0.402621     6.86849        0.287018        0.302798E-02
     7     973.963       0.10267E-02   -2.3336        0.358502     5.44568        0.303298        0.240073E-02
     8     1054.41       0.94840E-03  -0.15105        0.023205    0.228157E-01    0.303366        0.100583E-04
     9     1163.25       0.85966E-03   -1.0631        0.163325     1.13025        0.306745        0.498273E-03
    10     1208.51       0.82747E-03   0.99884        0.153448    0.997679        0.309727        0.439827E-03
    11     1293.74       0.77295E-03    2.9761        0.457212     8.85736        0.336205        0.390477E-02
    12     1494.09       0.66930E-03    2.1445        0.329457     4.59905        0.349953        0.202749E-02
    13     1583.46       0.63153E-03   -3.8613        0.593201     14.9098        0.394525        0.657300E-02
    14     1727.99       0.57871E-03   -6.0226        0.925231     36.2719        0.502955        0.159905E-01
    15     1801.91       0.55497E-03  -0.43217        0.066392    0.186767        0.503513        0.823362E-04
    16     1861.88       0.53709E-03   0.38773        0.059565    0.150334        0.503963        0.662748E-04
    17     1899.56       0.52644E-03  -0.65828E-01    0.010113    0.433332E-02    0.503976        0.191035E-05
    18     1972.34       0.50701E-03   -2.0794        0.319449     4.32387        0.516902        0.190618E-02
    19     2229.88       0.44845E-03   -2.9305        0.450208     8.58809        0.542575        0.378607E-02
    20     2297.22       0.43531E-03   0.47622E-01    0.007316    0.226786E-02    0.542581        0.999785E-06
    21     2332.39       0.42874E-03    1.0256        0.157551     1.05175        0.545726        0.463666E-03
    22     2398.97       0.41685E-03   -6.2645        0.962392     39.2440        0.663041        0.173007E-01
    23     2587.42       0.38649E-03   0.30837        0.047374    0.950940E-01    0.663325        0.419222E-04
    24     2590.78       0.38598E-03   0.15547E-02    0.000239    0.241720E-05    0.663325        0.106563E-08
    25     2603.41       0.38411E-03    1.9982        0.306977     3.99284        0.675261        0.176025E-02
    26     2612.83       0.38273E-03   0.24382        0.037457    0.594482E-01    0.675439        0.262078E-04
    27     2633.61       0.37971E-03   0.63409E-01    0.009741    0.402072E-02    0.675451        0.177254E-05
    28     2636.68       0.37926E-03    1.5492        0.238000     2.40007        0.682626        0.105807E-02
    29     2697.77       0.37068E-03   -2.1564        0.331275     4.64994        0.696526        0.204993E-02
    30     2708.84       0.36916E-03   0.35716        0.054868    0.127560        0.696908        0.562350E-04
    31     2739.75       0.36500E-03  -0.23165E-02    0.000356    0.536614E-05    0.696908        0.236567E-08
    32     2798.04       0.35739E-03   -2.5344        0.389345     6.42302        0.716108        0.283159E-02
    33     2824.74       0.35402E-03  -0.71947E-01    0.011053    0.517643E-02    0.716124        0.228203E-05
    34     2872.96       0.34807E-03   0.52375        0.080462    0.274319        0.716944        0.120934E-03
    35     2874.93       0.34784E-03  -0.17144        0.026338    0.293919E-01    0.717032        0.129574E-04
    36     2916.27       0.34290E-03  -0.10132        0.015565    0.102652E-01    0.717063        0.452540E-05
    37     3006.32       0.33263E-03    2.0441        0.314033     4.17850        0.729554        0.184210E-02
    38     3066.61       0.32609E-03   0.56391E-01    0.008663    0.317999E-02    0.729563        0.140190E-05
    39     3197.70       0.31273E-03   0.29470        0.045274    0.868510E-01    0.729823        0.382883E-04
    40     3269.98       0.30581E-03   0.59526        0.091448    0.354338        0.730882        0.156210E-03
    41     3326.72       0.30060E-03   0.82224        0.126318    0.676083        0.732903        0.298051E-03
    42     3343.11       0.29912E-03  -0.55599        0.085415    0.309127        0.733827        0.136279E-03
    43     3392.48       0.29477E-03   -3.6172        0.555694     13.0840        0.772940        0.576810E-02
    44     3418.08       0.29256E-03   0.40438        0.062123    0.163519        0.773429        0.720876E-04
    45     3597.73       0.27795E-03   0.49661        0.076292    0.246623        0.774166        0.108724E-03
    46     3631.50       0.27537E-03  -0.21856        0.033577    0.477703E-01    0.774309        0.210595E-04
    47     3645.56       0.27431E-03  -0.48216        0.074072    0.232474        0.775004        0.102486E-03
    48     3719.01       0.26889E-03    1.2849        0.197401     1.65108        0.779940        0.727878E-03
    49     3777.36       0.26474E-03   -1.6149        0.248088     2.60783        0.787736        0.114967E-02
    50     3798.28       0.26328E-03  -0.11140E-01    0.001711    0.124095E-03    0.787736        0.547074E-07
    51     3846.78       0.25996E-03   -4.0419        0.620949     16.3373        0.836575        0.720233E-02
    52     3864.14       0.25879E-03    2.4544        0.377057     6.02397        0.854583        0.265567E-02
    53     3871.49       0.25830E-03    1.2127        0.186305     1.47068        0.858979        0.648348E-03
    54     3902.39       0.25625E-03  -0.28385E-01    0.004361    0.805696E-03    0.858981        0.355192E-06
    55     3906.77       0.25597E-03    1.3433        0.206367     1.80447        0.864376        0.795500E-03
    56     4117.04       0.24289E-03    1.1148        0.171267     1.24284        0.868091        0.547907E-03
    57     4135.43       0.24181E-03   0.38738E-01    0.005951    0.150065E-02    0.868096        0.661564E-06
    58     4241.40       0.23577E-03    1.3936        0.214090     1.94206        0.873901        0.856157E-03
    59     4320.31       0.23146E-03  -0.64901        0.099705    0.421214        0.875160        0.185693E-03
    60     4431.34       0.22567E-03   0.12798        0.019662    0.163797E-01    0.875209        0.722102E-05
    61     4492.87       0.22257E-03  -0.85376        0.131160    0.728903        0.877388        0.321337E-03
    62     4515.70       0.22145E-03    1.6395        0.251873     2.68803        0.885424        0.118502E-02
    63     4534.65       0.22052E-03   -2.0141        0.309413     4.05646        0.897550        0.178829E-02
    64     4668.02       0.21422E-03  -0.26528        0.040753    0.703708E-01    0.897760        0.310230E-04
    65     4757.33       0.21020E-03  -0.60418E-01    0.009282    0.365028E-02    0.897771        0.160923E-05
    66     4849.75       0.20620E-03   -1.2699        0.195084     1.61255        0.902592        0.710894E-03
    67     4977.68       0.20090E-03    1.1459        0.176037     1.31304        0.906517        0.578853E-03
    68     5097.86       0.19616E-03   -1.8929        0.290796     3.58299        0.917228        0.157956E-02
    69     5120.83       0.19528E-03    2.6491        0.406964     7.01750        0.938206        0.309367E-02
    70     5203.70       0.19217E-03   0.15165        0.023298    0.229983E-01    0.938275        0.101388E-04
    71     5255.31       0.19028E-03   -1.6955        0.260469     2.87462        0.946868        0.126728E-02
    72     5297.84       0.18876E-03  -0.14160        0.021754    0.200519E-01    0.946928        0.883991E-05
    73     5337.33       0.18736E-03  -0.61490        0.094465    0.378101        0.948058        0.166686E-03
    74     5346.91       0.18702E-03   0.19766        0.030366    0.390693E-01    0.948175        0.172237E-04
    75     5359.22       0.18659E-03  -0.12738E-01    0.001957    0.162250E-03    0.948176        0.715278E-07
    76     5365.17       0.18639E-03   0.32177E-01    0.004943    0.103534E-02    0.948179        0.456431E-06
    77     5374.00       0.18608E-03  -0.19790        0.030403    0.391662E-01    0.948296        0.172664E-04
    78     5382.09       0.18580E-03  -0.41685E-01    0.006404    0.173763E-02    0.948301        0.766036E-06
    79     5400.38       0.18517E-03   0.71447        0.109762    0.510473        0.949827        0.225042E-03
    80     5422.67       0.18441E-03   0.60362        0.092732    0.364358        0.950916        0.160627E-03
    81     5465.45       0.18297E-03  -0.58017E-02    0.000891    0.336595E-04    0.950916        0.148388E-07
    82     5485.45       0.18230E-03  -0.30480E-01    0.004683    0.929045E-03    0.950919        0.409570E-06
    83     5516.43       0.18128E-03   0.90065        0.138364    0.811173        0.953344        0.357606E-03
    84     5578.06       0.17927E-03  -0.88180E-01    0.013547    0.777569E-02    0.953367        0.342791E-05
    85     5588.39       0.17894E-03    1.0350        0.158998     1.07115        0.956569        0.472217E-03
    86     5650.59       0.17697E-03   -1.0639        0.163444     1.13190        0.959953        0.498999E-03
    87     5699.52       0.17545E-03    1.5305        0.235126     2.34245        0.966955        0.103267E-02
    88     5786.97       0.17280E-03    1.6650        0.255782     2.77210        0.975242        0.122208E-02
    89     5834.33       0.17140E-03  -0.34530E-01    0.005305    0.119234E-02    0.975246        0.525643E-06
    90     5854.07       0.17082E-03  -0.13030        0.020017    0.169778E-01    0.975297        0.748466E-05
    91     5885.73       0.16990E-03   0.71231E-01    0.010943    0.507383E-02    0.975312        0.223680E-05
    92     6014.12       0.16628E-03   0.10554        0.016214    0.111386E-01    0.975345        0.491044E-05
    93     6093.25       0.16412E-03   0.12681E-01    0.001948    0.160796E-03    0.975346        0.708870E-07
    94     6126.76       0.16322E-03   0.62536        0.096072    0.391075        0.976515        0.172405E-03
    95     6214.32       0.16092E-03  -0.63108        0.096951    0.398267        0.977705        0.175576E-03
    96     6296.43       0.15882E-03   0.29769        0.045732    0.886174E-01    0.977970        0.390670E-04
    97     6320.07       0.15823E-03   0.81340        0.124959    0.661615        0.979948        0.291673E-03
    98     6431.11       0.15549E-03   -2.4477        0.376024     5.99102        0.997857        0.264114E-02
    99     6448.74       0.15507E-03   0.70482        0.108279    0.496776        0.999342        0.219004E-03
   100     6460.04       0.15480E-03  -0.46900        0.072051    0.219965         1.00000        0.969718E-04
 -----------------------------------------------------------------------------------------------------------------
   sum                                                             334.517                        0.147472    
 -----------------------------------------------------------------------------------------------------------------

          ***** PARTICIPATION FACTOR CALCULATION *****ROTY DIRECTION
                                                                                  CUMULATIVE     RATIO EFF.MASS
  MODE   FREQUENCY       PERIOD      PARTIC.FACTOR     RATIO    EFFECTIVE MASS   MASS FRACTION   TO TOTAL MASS
     1     573.242       0.17445E-02    19.597        1.000000     384.028        0.571791        0.168407    
     2     607.660       0.16457E-02    2.1014        0.107232     4.41584        0.578366        0.193647E-02
     3     841.842       0.11879E-02  -0.64634E-01    0.003298    0.417750E-02    0.578372        0.183195E-05
     4     869.973       0.11495E-02   0.14940        0.007624    0.223194E-01    0.578406        0.978765E-05
     5     903.975       0.11062E-02   0.91801E-01    0.004685    0.842748E-02    0.578418        0.369568E-05
     6     909.421       0.10996E-02   0.37381E-01    0.001908    0.139734E-02    0.578420        0.612769E-06
     7     973.963       0.10267E-02  -0.47627E-01    0.002430    0.226835E-02    0.578424        0.994732E-06
     8     1054.41       0.94840E-03   0.10747        0.005484    0.115504E-01    0.578441        0.506517E-05
     9     1163.25       0.85966E-03   0.50005        0.025517    0.250050        0.578813        0.109654E-03
    10     1208.51       0.82747E-03    9.6734        0.493625     93.5745        0.718139        0.410349E-01
    11     1293.74       0.77295E-03   -1.0552        0.053845     1.11342        0.719797        0.488263E-03
    12     1494.09       0.66930E-03  -0.26304        0.013423    0.691897E-01    0.719900        0.303415E-04
    13     1583.46       0.63153E-03   0.24564        0.012535    0.603373E-01    0.719990        0.264595E-04
    14     1727.99       0.57871E-03   0.46008        0.023477    0.211670        0.720305        0.928232E-04
    15     1801.91       0.55497E-03   0.52641E-01    0.002686    0.277109E-02    0.720309        0.121520E-05
    16     1861.88       0.53709E-03  -0.39908        0.020365    0.159268        0.720546        0.698435E-04
    17     1899.56       0.52644E-03   -3.7914        0.193471     14.3746        0.741949        0.630366E-02
    18     1972.34       0.50701E-03  -0.64102        0.032711    0.410910        0.742561        0.180195E-03
    19     2229.88       0.44845E-03  -0.35619E-01    0.001818    0.126875E-02    0.742563        0.556380E-06
    20     2297.22       0.43531E-03    5.0362        0.256993     25.3632        0.780327        0.111224E-01
    21     2332.39       0.42874E-03    1.8956        0.096729     3.59317        0.785677        0.157570E-02
    22     2398.97       0.41685E-03   0.30819        0.015727    0.949824E-01    0.785818        0.416524E-04
    23     2587.42       0.38649E-03  -0.37782        0.019280    0.142748        0.786031        0.625991E-04
    24     2590.78       0.38598E-03  -0.51402E-01    0.002623    0.264218E-02    0.786035        0.115867E-05
    25     2603.41       0.38411E-03   0.20094        0.010254    0.403768E-01    0.786095        0.177063E-04
    26     2612.83       0.38273E-03   -1.0337        0.052746     1.06844        0.787686        0.468538E-03
    27     2633.61       0.37971E-03  -0.43320        0.022106    0.187665        0.787965        0.822961E-04
    28     2636.68       0.37926E-03   0.22780        0.011624    0.518929E-01    0.788042        0.227565E-04
    29     2697.77       0.37068E-03   0.29189        0.014895    0.851990E-01    0.788169        0.373621E-04
    30     2708.84       0.36916E-03   -1.6812        0.085789     2.82634        0.792377        0.123943E-02
    31     2739.75       0.36500E-03   0.42243        0.021556    0.178443        0.792643        0.782521E-04
    32     2798.04       0.35739E-03   0.16624        0.008483    0.276348E-01    0.792684        0.121186E-04
    33     2824.74       0.35402E-03    2.1267        0.108524     4.52291        0.799418        0.198342E-02
    34     2872.96       0.34807E-03  -0.44299        0.022606    0.196244        0.799711        0.860582E-04
    35     2874.93       0.34784E-03  -0.89738        0.045792    0.805286        0.800910        0.353140E-03
    36     2916.27       0.34290E-03   -1.4880        0.075933     2.21422        0.804206        0.970993E-03
    37     3006.32       0.33263E-03   0.17328        0.008843    0.300272E-01    0.804251        0.131677E-04
    38     3066.61       0.32609E-03    1.7666        0.090150     3.12102        0.808898        0.136865E-02
    39     3197.70       0.31273E-03    4.3948        0.224262     19.3140        0.837655        0.846973E-02
    40     3269.98       0.30581E-03    4.0537        0.206857     16.4324        0.862122        0.720607E-02
    41     3326.72       0.30060E-03    2.2678        0.115723     5.14285        0.869780        0.225528E-02
    42     3343.11       0.29912E-03  -0.68507        0.034958    0.469318        0.870478        0.205809E-03
    43     3392.48       0.29477E-03    1.8105        0.092388     3.27792        0.875359        0.143746E-02
    44     3418.08       0.29256E-03    1.2273        0.062630     1.50638        0.877602        0.660587E-03
    45     3597.73       0.27795E-03    3.4508        0.176091     11.9080        0.895332        0.522198E-02
    46     3631.50       0.27537E-03  -0.16184        0.008259    0.261933E-01    0.895371        0.114865E-04
    47     3645.56       0.27431E-03   -3.0113        0.153662     9.06763        0.908872        0.397640E-02
    48     3719.01       0.26889E-03    1.9831        0.101198     3.93281        0.914728        0.172464E-02
    49     3777.36       0.26474E-03   0.78299        0.039955    0.613070        0.915641        0.268848E-03
    50     3798.28       0.26328E-03   0.78054        0.039830    0.609245        0.916548        0.267170E-03
    51     3846.78       0.25996E-03   0.91316        0.046598    0.833857        0.917789        0.365669E-03
    52     3864.14       0.25879E-03  -0.35020        0.017870    0.122639        0.917972        0.537807E-04
    53     3871.49       0.25830E-03  -0.18366        0.009372    0.337306E-01    0.918022        0.147918E-04
    54     3902.39       0.25625E-03  -0.40712E-02    0.000208    0.165750E-04    0.918022        0.726859E-08
    55     3906.77       0.25597E-03  -0.19927        0.010169    0.397103E-01    0.918081        0.174140E-04
    56     4117.04       0.24289E-03   0.77690        0.039644    0.603566        0.918980        0.264680E-03
    57     4135.43       0.24181E-03   -1.1746        0.059938     1.37966        0.921034        0.605017E-03
    58     4241.40       0.23577E-03   0.16920        0.008634    0.286294E-01    0.921077        0.125548E-04
    59     4320.31       0.23146E-03   -3.8756        0.197767     15.0201        0.943441        0.658671E-02
    60     4431.34       0.22567E-03    1.0742        0.054817     1.15397        0.945159        0.506048E-03
    61     4492.87       0.22257E-03   0.22703        0.011585    0.515436E-01    0.945235        0.226033E-04
    62     4515.70       0.22145E-03  -0.41891        0.021376    0.175482        0.945497        0.769535E-04
    63     4534.65       0.22052E-03    1.0198        0.052041     1.04003        0.947045        0.456081E-03
    64     4668.02       0.21422E-03  -0.55243E-01    0.002819    0.305177E-02    0.947050        0.133829E-05
    65     4757.33       0.21020E-03  -0.18705        0.009545    0.349891E-01    0.947102        0.153436E-04
    66     4849.75       0.20620E-03   0.27457        0.014011    0.753901E-01    0.947214        0.330606E-04
    67     4977.68       0.20090E-03    3.5977        0.183587     12.9433        0.966486        0.567599E-02
    68     5097.86       0.19616E-03   0.92635        0.047271    0.858125        0.967764        0.376311E-03
    69     5120.83       0.19528E-03  -0.80990        0.041328    0.655932        0.968740        0.287644E-03
    70     5203.70       0.19217E-03   0.19283        0.009840    0.371818E-01    0.968796        0.163052E-04
    71     5255.31       0.19028E-03  -0.23382        0.011932    0.546741E-01    0.968877        0.239761E-04
    72     5297.84       0.18876E-03   0.75677E-01    0.003862    0.572699E-02    0.968886        0.251144E-05
    73     5337.33       0.18736E-03  -0.87746E-01    0.004478    0.769934E-02    0.968897        0.337637E-05
    74     5346.91       0.18702E-03   0.67328E-01    0.003436    0.453300E-02    0.968904        0.198784E-05
    75     5359.22       0.18659E-03   0.27036E-01    0.001380    0.730919E-03    0.968905        0.320528E-06
    76     5365.17       0.18639E-03   0.12384E-01    0.000632    0.153367E-03    0.968905        0.672557E-07
    77     5374.00       0.18608E-03  -0.24612E-01    0.001256    0.605775E-03    0.968906        0.265649E-06
    78     5382.09       0.18580E-03  -0.17758E-01    0.000906    0.315347E-03    0.968906        0.138288E-06
    79     5400.38       0.18517E-03   0.10765        0.005493    0.115875E-01    0.968924        0.508143E-05
    80     5422.67       0.18441E-03   0.15501        0.007910    0.240275E-01    0.968959        0.105367E-04
    81     5465.45       0.18297E-03  -0.62026        0.031651    0.384724        0.969532        0.168712E-03
    82     5485.45       0.18230E-03   -1.0988        0.056073     1.20744        0.971330        0.529495E-03
    83     5516.43       0.18128E-03  -0.11868E-01    0.000606    0.140845E-03    0.971330        0.617642E-07
    84     5578.06       0.17927E-03   0.89107E-01    0.004547    0.794006E-02    0.971342        0.348193E-05
    85     5588.39       0.17894E-03  -0.27331        0.013947    0.747002E-01    0.971453        0.327580E-04
    86     5650.59       0.17697E-03   -2.8216        0.143986     7.96170        0.983308        0.349142E-02
    87     5699.52       0.17545E-03  -0.93899        0.047916    0.881705        0.984621        0.386651E-03
    88     5786.97       0.17280E-03  -0.78233        0.039922    0.612044        0.985532        0.268398E-03
    89     5834.33       0.17140E-03   0.16396        0.008367    0.268840E-01    0.985572        0.117894E-04
    90     5854.07       0.17082E-03   0.31808        0.016231    0.101175        0.985722        0.443681E-04
    91     5885.73       0.16990E-03   0.74616        0.038076    0.556761        0.986551        0.244155E-03
    92     6014.12       0.16628E-03   0.12169        0.006210    0.148093E-01    0.986574        0.649427E-05
    93     6093.25       0.16412E-03  -0.18779E-01    0.000958    0.352639E-03    0.986574        0.154642E-06
    94     6126.76       0.16322E-03  -0.24668        0.012588    0.608524E-01    0.986665        0.266854E-04
    95     6214.32       0.16092E-03   0.22545        0.011504    0.508256E-01    0.986740        0.222884E-04
    96     6296.43       0.15882E-03   0.74565        0.038050    0.555999        0.987568        0.243821E-03
    97     6320.07       0.15823E-03    2.7355        0.139588     7.48269        0.998709        0.328136E-02
    98     6431.11       0.15549E-03   0.90716        0.046292    0.822947        0.999935        0.360885E-03
    99     6448.74       0.15507E-03  -0.12730        0.006496    0.162053E-01    0.999959        0.710645E-05
   100     6460.04       0.15480E-03  -0.16628        0.008485    0.276503E-01     1.00000        0.121254E-04
 -----------------------------------------------------------------------------------------------------------------
   sum                                                             671.623                        0.294525    
 -----------------------------------------------------------------------------------------------------------------

          ***** PARTICIPATION FACTOR CALCULATION *****ROTZ DIRECTION
                                                                                  CUMULATIVE     RATIO EFF.MASS
  MODE   FREQUENCY       PERIOD      PARTIC.FACTOR     RATIO    EFFECTIVE MASS   MASS FRACTION   TO TOTAL MASS
     1     573.242       0.17445E-02  -0.79450        0.752077    0.631228        0.199635        0.259951E-01
     2     607.660       0.16457E-02  -0.85171E-01    0.080623    0.725409E-02    0.201929        0.298737E-03
     3     841.842       0.11879E-02  -0.16967E-02    0.001606    0.287884E-05    0.201930        0.118556E-06
     4     869.973       0.11495E-02  -0.29414E-02    0.002784    0.865203E-05    0.201932        0.356307E-06
     5     903.975       0.11062E-02  -0.10199E-02    0.000965    0.104019E-05    0.201933        0.428371E-07
     6     909.421       0.10996E-02  -0.84582E-03    0.000801    0.715410E-06    0.201933        0.294619E-07
     7     973.963       0.10267E-02  -0.49054E-02    0.004644    0.240632E-04    0.201941        0.990968E-06
     8     1054.41       0.94840E-03  -0.10348E-01    0.009795    0.107072E-03    0.201974        0.440941E-05
     9     1163.25       0.85966E-03   0.17820E-01    0.016868    0.317549E-03    0.202075        0.130773E-04
    10     1208.51       0.82747E-03   0.70976        0.671864    0.503761        0.361397        0.207458E-01
    11     1293.74       0.77295E-03  -0.59458E-01    0.056283    0.353520E-02    0.362515        0.145586E-03
    12     1494.09       0.66930E-03   0.24593E-01    0.023280    0.604829E-03    0.362706        0.249080E-04
    13     1583.46       0.63153E-03  -0.11717E-01    0.011091    0.137280E-03    0.362749        0.565346E-05
    14     1727.99       0.57871E-03  -0.20915E-01    0.019798    0.437425E-03    0.362888        0.180140E-04
    15     1801.91       0.55497E-03  -0.17111E-01    0.016197    0.292788E-03    0.362980        0.120576E-04
    16     1861.88       0.53709E-03   0.27657E-01    0.026181    0.764935E-03    0.363222        0.315014E-04
    17     1899.56       0.52644E-03    1.0564        1.000000     1.11599        0.716171        0.459587E-01
    18     1972.34       0.50701E-03   0.19169        0.181456    0.367456E-01    0.727792        0.151325E-02
    19     2229.88       0.44845E-03  -0.44966E-01    0.042565    0.202190E-02    0.728431        0.832657E-04
    20     2297.22       0.43531E-03  -0.15145        0.143361    0.229362E-01    0.735685        0.944555E-03
    21     2332.39       0.42874E-03  -0.20619E-01    0.019518    0.425146E-03    0.735820        0.175083E-04
    22     2398.97       0.41685E-03  -0.34121E-02    0.003230    0.116422E-04    0.735823        0.479447E-06
    23     2587.42       0.38649E-03   0.42600E-01    0.040325    0.181474E-02    0.736397        0.747345E-04
    24     2590.78       0.38598E-03   0.16750E-01    0.015855    0.280547E-03    0.736486        0.115534E-04
    25     2603.41       0.38411E-03  -0.35607E-01    0.033706    0.126786E-02    0.736887        0.522128E-04
    26     2612.83       0.38273E-03   0.12315        0.116573    0.151656E-01    0.741683        0.624546E-03
    27     2633.61       0.37971E-03   0.14856E-01    0.014063    0.220708E-03    0.741753        0.908915E-05
    28     2636.68       0.37926E-03  -0.12801E-01    0.012117    0.163856E-03    0.741805        0.674788E-05
    29     2697.77       0.37068E-03   0.13366E-01    0.012652    0.178638E-03    0.741862        0.735665E-05
    30     2708.84       0.36916E-03   0.17939        0.169815    0.321819E-01    0.752040        0.132531E-02
    31     2739.75       0.36500E-03  -0.21478E-01    0.020331    0.461308E-03    0.752185        0.189975E-04
    32     2798.04       0.35739E-03   0.65164E-02    0.006168    0.424633E-04    0.752199        0.174872E-05
    33     2824.74       0.35402E-03  -0.89589E-01    0.084806    0.802627E-02    0.754737        0.330536E-03
    34     2872.96       0.34807E-03   0.10280E-01    0.009731    0.105672E-03    0.754771        0.435179E-05
    35     2874.93       0.34784E-03   0.12090E-01    0.011444    0.146162E-03    0.754817        0.601920E-05
    36     2916.27       0.34290E-03   0.19917        0.188531    0.396667E-01    0.767362        0.163355E-02
    37     3006.32       0.33263E-03  -0.82092E-02    0.007771    0.673917E-04    0.767383        0.277531E-05
    38     3066.61       0.32609E-03  -0.56022E-01    0.053031    0.313847E-02    0.768376        0.129248E-03
    39     3197.70       0.31273E-03  -0.35752        0.338427    0.127818        0.808800        0.526379E-02
    40     3269.98       0.30581E-03  -0.14569        0.137909    0.212248E-01    0.815513        0.874077E-03
    41     3326.72       0.30060E-03  -0.16589        0.157035    0.275204E-01    0.824217        0.113334E-02
    42     3343.11       0.29912E-03   0.58720E-01    0.055585    0.344808E-02    0.825307        0.141998E-03
    43     3392.48       0.29477E-03  -0.10125        0.095844    0.102515E-01    0.828549        0.422177E-03
    44     3418.08       0.29256E-03   0.29334E-01    0.027768    0.860496E-03    0.828821        0.354368E-04
    45     3597.73       0.27795E-03   0.38835        0.367617    0.150818        0.876520        0.621095E-02
    46     3631.50       0.27537E-03   0.40224E-01    0.038076    0.161796E-02    0.877031        0.666305E-04
    47     3645.56       0.27431E-03  -0.11875E-02    0.001124    0.141004E-05    0.877032        0.580681E-07
    48     3719.01       0.26889E-03  -0.34986        0.331181    0.122403        0.915743        0.504080E-02
    49     3777.36       0.26474E-03  -0.38380E-01    0.036331    0.147305E-02    0.916209        0.606631E-04
    50     3798.28       0.26328E-03  -0.60843E-01    0.057595    0.370192E-02    0.917380        0.152452E-03
    51     3846.78       0.25996E-03  -0.39928E-01    0.037796    0.159424E-02    0.917884        0.656539E-04
    52     3864.14       0.25879E-03   0.18623E-01    0.017628    0.346802E-03    0.917994        0.142820E-04
    53     3871.49       0.25830E-03   0.19063E-02    0.001804    0.363385E-05    0.917995        0.149648E-06
    54     3902.39       0.25625E-03   0.16920E-01    0.016016    0.286277E-03    0.918086        0.117894E-04
    55     3906.77       0.25597E-03   0.10656E-01    0.010087    0.113551E-03    0.918122        0.467623E-05
    56     4117.04       0.24289E-03  -0.37880E-01    0.035858    0.143491E-02    0.918575        0.590920E-04
    57     4135.43       0.24181E-03   0.13896        0.131539    0.193095E-01    0.924682        0.795199E-03
    58     4241.40       0.23577E-03  -0.36166E-02    0.003424    0.130800E-04    0.924686        0.538660E-06
    59     4320.31       0.23146E-03   0.14996        0.141954    0.224884E-01    0.931799        0.926112E-03
    60     4431.34       0.22567E-03  -0.40434E-01    0.038275    0.163492E-02    0.932316        0.673292E-04
    61     4492.87       0.22257E-03   0.45633E-02    0.004320    0.208236E-04    0.932322        0.857555E-06
    62     4515.70       0.22145E-03   0.24338E-01    0.023038    0.592332E-03    0.932510        0.243933E-04
    63     4534.65       0.22052E-03  -0.41144E-01    0.038948    0.169286E-02    0.933045        0.697151E-04
    64     4668.02       0.21422E-03   0.91052E-03    0.000862    0.829052E-06    0.933045        0.341419E-07
    65     4757.33       0.21020E-03   0.15527        0.146977    0.241079E-01    0.940670        0.992807E-03
    66     4849.75       0.20620E-03  -0.14941E-01    0.014143    0.223235E-03    0.940740        0.919321E-05
    67     4977.68       0.20090E-03  -0.42394E-01    0.040131    0.179727E-02    0.941309        0.740148E-04
    68     5097.86       0.19616E-03  -0.42259E-01    0.040002    0.178579E-02    0.941874        0.735421E-04
    69     5120.83       0.19528E-03  -0.13999E-01    0.013252    0.195972E-03    0.941936        0.807047E-05
    70     5203.70       0.19217E-03   0.90106E-02    0.008529    0.811909E-04    0.941961        0.334359E-05
    71     5255.31       0.19028E-03  -0.33210E-02    0.003144    0.110290E-04    0.941965        0.454194E-06
    72     5297.84       0.18876E-03   0.39463        0.373559    0.155732        0.991217        0.641335E-02
    73     5337.33       0.18736E-03   0.14567E-01    0.013789    0.212202E-03    0.991284        0.873886E-05
    74     5346.91       0.18702E-03  -0.48385E-02    0.004580    0.234112E-04    0.991292        0.964117E-06
    75     5359.22       0.18659E-03   0.55714E-03    0.000527    0.310403E-06    0.991292        0.127830E-07
    76     5365.17       0.18639E-03  -0.11078E-04    0.000010    0.122721E-09    0.991292        0.505387E-11
    77     5374.00       0.18608E-03   0.14338E-02    0.001357    0.205573E-05    0.991293        0.846588E-07
    78     5382.09       0.18580E-03  -0.10017E-02    0.000948    0.100346E-05    0.991293        0.413242E-07
    79     5400.38       0.18517E-03  -0.73095E-03    0.000692    0.534295E-06    0.991293        0.220032E-07
    80     5422.67       0.18441E-03   0.37809E-02    0.003579    0.142950E-04    0.991298        0.588695E-06
    81     5465.45       0.18297E-03   0.18401E-01    0.017418    0.338594E-03    0.991405        0.139439E-04
    82     5485.45       0.18230E-03   0.70302E-01    0.066548    0.494235E-02    0.992968        0.203535E-03
    83     5516.43       0.18128E-03  -0.50657E-02    0.004795    0.256613E-04    0.992976        0.105678E-05
    84     5578.06       0.17927E-03  -0.23697E-02    0.002243    0.561562E-05    0.992978        0.231262E-06
    85     5588.39       0.17894E-03   0.45940E-02    0.004349    0.211053E-04    0.992984        0.869154E-06
    86     5650.59       0.17697E-03   0.55947E-01    0.052959    0.313002E-02    0.993974        0.128900E-03
    87     5699.52       0.17545E-03   0.25036E-01    0.023699    0.626806E-03    0.994172        0.258130E-04
    88     5786.97       0.17280E-03   0.25714E-01    0.024341    0.661189E-03    0.994382        0.272290E-04
    89     5834.33       0.17140E-03  -0.40206E-02    0.003806    0.161652E-04    0.994387        0.665711E-06
    90     5854.07       0.17082E-03  -0.16099E-01    0.015239    0.259177E-03    0.994469        0.106734E-04
    91     5885.7
```
