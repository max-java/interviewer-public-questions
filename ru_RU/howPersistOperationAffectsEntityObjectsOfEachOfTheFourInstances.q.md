![tag](https://img.shields.io/badge/language-java-red.svg)   ![tag](https://img.shields.io/badge/jdk-1.8-blue.svg)     ![tag](https://img.shields.io/badge/level-L1-green.svg)     ![tag](https://img.shields.io/badge/topic-JPA-green.svg)      ![tag](https://img.shields.io/badge/locale-ru-green.svg)     ![question](https://img.shields.io/badge/-question-grey.svg) 

# Как влияет операция persist на Entity объекты каждого из статусов жизненного цикла Entity объекта?
> 
* Если статус Entity **new**, то он меняется на managed и объект будет сохранен в базу при коммите транзакции или в результате flush операций.
* Если статус **managed**, операция игнорируется, однако зависимые Entity могут поменять статус на managed, если у них есть аннотации каскадных изменений.
* Если статус **removed**, то он меняется на managed.
* Если статус **detached**, будет выкинут exception сразу или на этапе коммита транзакции.

![meta](https://img.shields.io/badge/_meta-red.svg)    ![id](https://img.shields.io/badge/_id-null-red.svg)    ![key](https://img.shields.io/badge/key-22c6bd811392459fa10f14dcf6c2b583-yellow.svg)    ![template_name](https://img.shields.io/badge/simple_question-v.0.1-yellow.svg)
