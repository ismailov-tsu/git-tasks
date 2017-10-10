# Задание 1

В [репозитории](https://git.bw-sw.com/education/git/git-flow) есть три ветки:

* `master` - стабильная версия проекта
* `develop` - текущая версия проекта для разработки
* `feature/D-42` - ветка проекта для разработки задачи D-42

Ветка `develop` не содержит изменений относительно ветки `master` и имеет следующую историю коммитов:

```bash
* 0ea4ad889269a879feede3c303205f2793d22908 Add documentation of Get Started
* f45d68ce197ee4a9b698ef0a65868d3b30960f74 Add README.md
```

Ветка `feature/D-42` содержит готовую реализацию задачи D-42 и имеет следующую историю коммитов:

```bash
* 82d37b1e702a644d3c3337e0fe04a026f76c0e24 Add images user guide
* dce3a8511d7809674ba7c4e7388ddced6ef355ab add dockerfile user guide
* ec13451bd9d7e22283fc596dad586b2d04b4f12a Add installation for Debian
* 85eb1b959496bd16e32fc9236a71425460e05808 Add installation for Ubuntu
* e7b5b2590e5c4c4ec749d66f7318a15566f6736e Add installation for Mac
* 459af9c5180ed4273a21cee57b8baf6a5bfc1de9 Add nightly channel to README.md
* 0ea4ad889269a879feede3c303205f2793d22908 Add documentation of Get Started
* f45d68ce197ee4a9b698ef0a65868d3b30960f74 Add README.md
```

Все коммиты, начиная с `459af9c5180ed4273a21cee57b8baf6a5bfc1de9`, относятся к задаче D-42 и принадлежат только этой ветке, но их оформление считается некорректным.

Необходимо слить реализацию задачи D-42 в `develop`, предварительно подправив историю коммитов ветки `feature/D-42` следующим образом:

* удалить коммит `459af9c5180ed4273a21cee57b8baf6a5bfc1de9`
* коммиты `e7b5b2590e5c4c4ec749d66f7318a15566f6736e`, `85eb1b959496bd16e32fc9236a71425460e05808` и `ec13451bd9d7e22283fc596dad586b2d04b4f12` объединить в один с описанием `Add documentation of Installation`
* исправить описание коммита `dce3a8511d7809674ba7c4e7388ddced6ef355ab` на `Add dockerfile user guide`

Результат работы должен находиться в вашем приватном репозитории `git-task1` с двумя ветками:

* прежняя ветка `master`
* ветка `develop`, содержащая реализацию задачи D-42 со следующей историей коммитов:

```bash
* <commit hash>........................... Add images user guide
* <commit hash>........................... Add dockerfile user guide
* <commit hash>........................... Add documentation of Installation
* 0ea4ad889269a879feede3c303205f2793d22908 Add documentation of Get Started
* f45d68ce197ee4a9b698ef0a65868d3b30960f74 Add README.md
```
