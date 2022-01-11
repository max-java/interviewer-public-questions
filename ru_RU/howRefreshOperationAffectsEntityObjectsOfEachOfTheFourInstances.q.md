![tag](https://img.shields.io/badge/language-java-red.svg)   ![tag](https://img.shields.io/badge/jdk-1.8-blue.svg)     ![tag](https://img.shields.io/badge/level-L1-green.svg)     ![tag](https://img.shields.io/badge/topic-JPA-green.svg)      ![tag](https://img.shields.io/badge/locale-ru-green.svg)     ![question](https://img.shields.io/badge/-question-grey.svg) 

# Как влияет операция refresh на Entity объекты каждого из статусов жизненного цикла Entity объекта?
> 
* Если статус Entity **managed**, то в результате операции будут восстановленны все изменения из базы данных данного Entity, так же произойдет refresh всех каскадно зависимых объектов.
* Если статус **new**, **removed**, **detached**, то будет выкинут exception.

![meta](https://img.shields.io/badge/_meta-red.svg)    ![id](https://img.shields.io/badge/_id-null-red.svg)    ![key](https://img.shields.io/badge/key-22c6bd811392459fa10f14dcf6c2b583-yellow.svg)    ![template_name](https://img.shields.io/badge/simple_question-v.0.1-yellow.svg)
