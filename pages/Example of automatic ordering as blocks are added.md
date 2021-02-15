---
title: Example of automatic ordering as blocks are added
---

## Example of automatic ordering as blocks are added and changed

## 1. T1 contains N1

## 2. +S1,2,3 : N1,S1,2,3

## 3. +Q2.1,2.2,2.3,2.4 : Q1,2,3,4,N1,S2,1,3

## 4. +C1 + link to Q2.2: C1(1),Q1,3,4,N1,S2,1,3

## 5. +T2 + link to C1,Q2.4,S3 : T2(3),Q1,3,N1,S2,1

## 6. +Q2.3 categorized as E1 : T2(3),E1,Q1,N1,S2,1

## 7. +N2, link to E1: T2(3),E1(1),Q1,N1,S2,1

## 8. +N2 categorized as C2 : T2(3),C2(1),Q1,N1,S2,1 (E1 and C2 switch level)

## 9. +link to T1 : switching T2 and T1, T2 with all blocks inside T2 moves to first level, T1 with all blocks not in T2 becomes subtopic in T2

## #claim 
