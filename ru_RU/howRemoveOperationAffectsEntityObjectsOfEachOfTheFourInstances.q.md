![tag](https://img.shields.io/badge/language-java-red.svg)   ![tag](https://img.shields.io/badge/jdk-1.8-blue.svg)     ![tag](https://img.shields.io/badge/level-L1-green.svg)     ![tag](https://img.shields.io/badge/topic-JPA-green.svg)      ![tag](https://img.shields.io/badge/locale-ru-green.svg)     ![question](https://img.shields.io/badge/-question-grey.svg) 

# Как влияет операция remove на Entity объекты каждого из статусов жизненного цикла Entity объекта?
> 
* Если статус Entity **new**, операция игнорируется, однако зависимые Entity могут поменять статус на removed, если у них есть аннотации каскадных изменений и они имели статус managed.
* Если статус **managed**, то статус меняется на removed и запись объекта в базе данных будет удалена при коммите транзакции (так же произойдут операции remove для всех каскадно зависимых объектов).
* Если статус **removed**, то операция игнорируется.
* Если статус **detached**, то будет выкинут exception сразу или на этапу коммита транзакции.

![meta](https://img.shields.io/badge/_meta-red.svg)    ![id](https://img.shields.io/badge/_id-null-red.svg)    ![key](https://img.shields.io/badge/key-22c6bd811392459fa10f14dcf6c2b583-yellow.svg)    ![template_name](https://img.shields.io/badge/simple_question-v.0.1-yellow.svg)
