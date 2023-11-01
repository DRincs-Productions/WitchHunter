## Character
| Eng  | Russian  | Italian | French |
| ------------- | ------------- | ------------- | ------------- |
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
