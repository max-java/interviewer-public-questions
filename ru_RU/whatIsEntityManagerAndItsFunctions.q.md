![tag](https://img.shields.io/badge/language-java-red.svg)   ![tag](https://img.shields.io/badge/jdk-1.8-blue.svg)     ![tag](https://img.shields.io/badge/level-L1-green.svg)     ![tag](https://img.shields.io/badge/topic-JPA-green.svg)      ![tag](https://img.shields.io/badge/locale-ru-green.svg)     ![question](https://img.shields.io/badge/-question-grey.svg) 

# Что такое EntityManager и и какие у него основные функции?
> 
EntityManager это интерфейс, который описывает API для всех основный операций над Entity, получение данных и других сущностей JPA. По сути главный API для работы с JPA.
Основные операции:
* Для операций на Entity: **persist** (добавление Entity под управление JPA), **merge** (обновление), **remove** (удаление), **refresh** (обновление данных), **detach** (удаление из управления JPA), **lock** (блокирование Entity от изменений в других thread).
* Получение данных: **find** (поиск и получение Entity), **createQuery**, **createNamedQuery**, **createNativeQuery**, **contains**, **createStoredProcedureQuery**, **createNamedStoredProcedureQuery**.
* Получение других сущностей JPA: **getTransaction**, **getEntityManagerFactory**, **getCriteriaBuilder**, **getMetamodel**, **getDelegate**.
* Работа с EntityGraph: **createEntityGraph**, **getEntityGraph**.
* Общие операции над EntityManager или всеми Entities: **close**, **isOpen**, **setProperty**, **getProperties**, **clear**.

![meta](https://img.shields.io/badge/_meta-red.svg)    ![id](https://img.shields.io/badge/_id-null-red.svg)    ![key](https://img.shields.io/badge/key-22c6bd811392459fa10f14dcf6c2b583-yellow.svg)    ![template_name](https://img.shields.io/badge/simple_question-v.0.1-yellow.svg)
