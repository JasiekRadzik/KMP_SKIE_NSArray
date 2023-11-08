# KMP_SKIE_NSArray

This repository contains two demo projects, iOS and Android. 
It's goal is to help the kotlin multiplatform team to reproduce a bug that I found while using the SKIE plugin (https://skie.touchlab.co).
Too put it short:
TestRepository.getFlowTwoLevels() returns a Flow<FirstLevel<List<SomeItem>>>. 
On iOS side the List<SomeItem> is lost and the NSArray is shown. TestRepository.getFlowTwoLevels() returns SkieSwiftFlow<FirstLevel<NSArray>>.
FirstLevel and a SecondLevel are sealed classes. They're located in TestEntities.kt file. 
