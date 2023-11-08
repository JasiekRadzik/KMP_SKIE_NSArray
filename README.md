# KMP_SKIE_NSArray

This repository contains two demo projects, iOS and Android. 
It's goal is to help the kotlin multiplatform team to reproduce a bug that I found while using the SKIE plugin (https://skie.touchlab.co).
Too put it short:
On iOS side the return type of TestRepository.getFlowTwoLevels is broken. List of SomeItems is lost and the NSArray is shown.
FirstLevel and a SecondLevel are sealed classes. They're located in TestEntities.kt file. 
