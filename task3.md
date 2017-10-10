# Задание 3

Даны два репозитория, каждый из которых соответствует отдельному проекту:

* [репозиторий А](https://git.bw-sw.com/education/git/join-a) для проекта А
* [репозиторий B](https://git.bw-sw.com/education/git/join-b) для проекта Б

Проект А содержит следующую историю коммитов:

```bash
* eaeea06becc6d1178097778bce0a2338c77d0c60 Add installation for Debian
* 575126d2f57a20b3b1684432b90f322ff04aba10 Add installation for Ubuntu
* 29687d8fca626adf1e78ed3899c7d8b0e5675ace Add installation for Mac
* d690c49d346175ca1c70c655e0d284c308e420e8 Add README.md
```

Проект Б содержит следующую историю коммитов:

```bash
* 342201b3cd91f3219b057d463d10b94d45bfbee1 Add Get Started, Part 2
* 6df91582104200ef5a723d37118af3db60bf0bdf Add Get Started, Part 1
```

Необходимо объединить проекты в один репозиторий с сохранением истории коммитов, используя два кейса.

### Кейс первый

История коммитов обоих проектов не должна измениться (хэш коммитов не меняется), обе истории должны объединиться в общем коммите.

Репозиторий должен содержать следующую историю:

```bash
*   <commit hash>......................... <Commit description>
|\  
| * 342201b3cd91f3219b057d463d10b94d45bfbee1 Add Get Started, Part 2
| * 6df91582104200ef5a723d37118af3db60bf0bdf Add Get Started, Part 1
* eaeea06becc6d1178097778bce0a2338c77d0c60 Add installation for Debian
* 575126d2f57a20b3b1684432b90f322ff04aba10 Add installation for Ubuntu
* 29687d8fca626adf1e78ed3899c7d8b0e5675ace Add installation for Mac
* d690c49d346175ca1c70c655e0d284c308e420e8 Add README.md
```

Результат работы должен находиться в вашем приватном репозитории `git-task3-case1` с единственной веткой `master`.

### Кейс второй

История коммитов проекта А не должна измениться (хэш коммитов не меняется), необходимо добавить историю коммитов проекта Б к истории проекта А.

Репозиторий должен содержать следующую историю:

```bash
* <commit hash>........................... Add Get Started, Part 2
* <commit hash>........................... Add Get Started, Part 1
* eaeea06becc6d1178097778bce0a2338c77d0c60 Add installation for Debian
* 575126d2f57a20b3b1684432b90f322ff04aba10 Add installation for Ubuntu
* 29687d8fca626adf1e78ed3899c7d8b0e5675ace Add installation for Mac
* d690c49d346175ca1c70c655e0d284c308e420e8 Add README.md
```

Результат работы должен находиться в вашем приватном репозитории `git-task3-case2` с единственной веткой `master`.
