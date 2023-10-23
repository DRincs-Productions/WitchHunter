## Character
| Eng  | Russian  | Italian |
| ------------- | ------------- | ------------- |
| [Blunk](https://witch.fandom.com/wiki/Blunk) | Бланк | Blunk  |
| [Lord_Cedric](https://witch.fandom.com/wiki/Lord_Cedric)  | Седрик | Cedric  |
| [Taranee](https://witch.fandom.com/it/wiki/Taranee_Cook) | Тарани  | Taranee  |

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
