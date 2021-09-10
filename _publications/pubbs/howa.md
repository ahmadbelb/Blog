---
title: "APDL modal TEST "
excerpt: "Map is a <br/><img src='https://ahmadbelb.github.io/Blog/images/modal1.gif' Width= 250px  loop=infinite>"
collection: publications
permalink: /publication/howa
date: 2021-03-23
venue: 'AGU Advances'
paperurl: ''
citation: ''
---


# Table of contents
1. [Introduction](#introduction)
2. [Some paragraph](#paragraph1)
    1. [Sub paragraph](#subparagraph1)
3. [code ](#paragraph2)
## This is the introduction <a name="introduction"></a>
Some introduction text, formatted in heading 2 style

## Some paragraph <a name="paragraph1"></a>
# How to QA

This template explains our QA process for shipping bug-free software.
## Some paragraph <a name="paragraph1"></a>
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
## Another paragraph <a name="paragraph2"></a>
```fortran
nLines = 9
LineDiv = 2

!###########################################################################
! Everything above is implermented in MATLAB
!###########################################################################
! Change view and background colour
/view,,-1,1,-1
/VUP,1,-Z 
/eshape,1
/RGB,INDEX,100,100,100, 0   
/RGB,INDEX, 80, 80, 80,13   
/RGB,INDEX, 60, 60, 60,14   
/RGB,INDEX, 0, 0, 0,15  
/REPLOT

!---------------------------------------------------------------------------
! Keypoints
!---------------------------------------------------------------------------
! Sensor locations
K,  1,     0, 0, 0
K,  2, 1/9*L, 0, 0 
K,  3, 2/9*L, 0, 0 
K,  4, 3/9*L, 0, 0 
K,  5, 4/9*L, 0, 0
K,  6, 5/9*L, 0, 0 
K,  7, 6/9*L, 0, 0
K,  8, 7/9*L, 0, 0 
K,  9, 8/9*L, 0, 0
K, 10,     L, 0, 0
!---------------------------------------------------------------------------
! Lines bodies
!---------------------------------------------------------------------------
! Line bodies
L, 1, 2
L, 2, 3
L, 3, 4
L, 4, 5
L, 5, 6 			
L, 6, 7
L, 7, 8
L, 8, 9
L, 9,10
!---------------------------------------------------------------------------
! Types
!---------------------------------------------------------------------------
ET,1,BEAM188, 0, 0, 0  ! KEYOPT(3) linear shape functions
SECTYPE, 1, beam, HREC, HSS, 0 		
d = 0.1524 
b = 0.0508
t = 0.00478 
SECDATA, d, b, t, t, t, t			

ET, 1001, MASS21
R, 1001, mpoint, mpoint, mpoint	
	
!---------------------------------------------------------------------------
! Boundary conditions

```
