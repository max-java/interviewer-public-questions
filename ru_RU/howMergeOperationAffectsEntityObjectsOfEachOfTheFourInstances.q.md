![tag](https://img.shields.io/badge/language-java-red.svg)   ![tag](https://img.shields.io/badge/jdk-1.8-blue.svg)     ![tag](https://img.shields.io/badge/level-L1-green.svg)     ![tag](https://img.shields.io/badge/topic-JPA-green.svg)      ![tag](https://img.shields.io/badge/locale-ru-green.svg)     ![question](https://img.shields.io/badge/-question-grey.svg) 

# Как влияет операция merge на Entity объекты каждого из статусов жизненного цикла Entity объекта?
> 
* Если статус **detached**, то либо данные будут скопированы в существующей managed entity с тем же первичным ключом, либо создан новый managed в который скопируются данные.
* Если статус Entity **new**, то будет создан новый managed entity, в который будут скопированы данные прошлого объекта.
* Если статус **managed**, то операция игнорируется, однако операция merge сработает на каскадно зависимые Entity, если их статус не managed.
* Если статус **removed**, то будет выкинут exception сразу или на этапе коммита транзакции.

![meta](https://img.shields.io/badge/_meta-red.svg)    ![id](https://img.shields.io/badge/_id-null-red.svg)    ![key](https://img.shields.io/badge/key-22c6bd811392459fa10f14dcf6c2b583-yellow.svg)    ![template_name](https://img.shields.io/badge/simple_question-v.0.1-yellow.svg)
