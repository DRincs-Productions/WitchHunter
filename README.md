## Character
| Eng  | Russian  | Italian | French |
| ------------- | ------------- | ------------- | ------------- |
| [Blunk](https://witch.fandom.com/wiki/Blunk) | Бланк | Blunk  | |
| [Lord_Cedric](https://witch.fandom.com/wiki/Lord_Cedric)  | Седрик | Cedric  | |
| [Taranee](https://witch.fandom.com/wiki/Taranee_Cook) | Тарани  | Taranee  | |
| [Taranee Cook](https://witch.fandom.com/wiki/Taranee_Cook) | Тарани Кук | Taranee Cook | |
| [Hay Lin](https://witch.fandom.com/wiki/Hay_Lin) | Хай Лин  | Hay Lin  | |
| [Will](https://witch.fandom.com/wiki/Will_Vandom) | Вилл | Will | |
| [Guardians of Kandrakar](https://disney.fandom.com/wiki/Guardians_of_Kandrakar) | Стражницы завесы        !!!!or!!!!!      стражницами Завесы| Guardiane di Kandrakar | |
| [Guardians](https://disney.fandom.com/wiki/Guardians_of_Kandrakar) | стражницах | guardiane | |
| [Guardian of Kandrakar](https://disney.fandom.com/wiki/Guardians_of_Kandrakar) | Стражницей завесы | Guardiana di Kandrakar | |

## Insert Template in your Project

```shell
git checkout -b translations-templete
git checkout translations-templete
git config pull.rebase false
git pull https://github.com/DRincs-Productions/renpy-translations-templete.git tool-only --allow-unrelated-histories
git submodule update --init --recursive

```

At the end make a merge inside the arm of the project.

### Fix Common
```regex
    # renpy/common/(.*)
    old "###########"
    new "(.*)"
```

```regex
    # # renpy/common/(.*)
    # old "###########"
    # new "(.*)"
```

### Check if there are a text after "
```regex
"(.*)"(.)(.*)\n
```
