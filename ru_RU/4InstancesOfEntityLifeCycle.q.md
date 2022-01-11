![tag](https://img.shields.io/badge/language-java-red.svg)   ![tag](https://img.shields.io/badge/jdk-1.8-blue.svg)     ![tag](https://img.shields.io/badge/level-L1-green.svg)     ![tag](https://img.shields.io/badge/topic-JPA-green.svg)      ![tag](https://img.shields.io/badge/locale-ru-green.svg)     ![question](https://img.shields.io/badge/-question-grey.svg) 

# Назовите 4 статуса жизненного цикла Entity объекта.
> 
У Entity объекта существует 4 статуса жизненного цикла: **new**, **managed**, **detached**, **removed**.
* new - объект создан, но при этом еще не имеет сгенерированных первичных ключей и пока еще не сохранен в базе данных.
* managed - объект создан, управляется JPA, имеет сгенерированные первичные ключи.
* detached - объект был создан, но не управляется (или больше не управляется) JPA.
* removed - объект создан, управляется JPA, но будет удален после коммита транзакции.

![meta](https://img.shields.io/badge/_meta-red.svg)    ![id](https://img.shields.io/badge/_id-null-red.svg)    ![key](https://img.shields.io/badge/key-22c6bd811392459fa10f14dcf6c2b583-yellow.svg)    ![template_name](https://img.shields.io/badge/simple_question-v.0.1-yellow.svg)
