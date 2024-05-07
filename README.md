## Notes

customize workflow only triger when it's open, also setup multiple action added

[link](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows)


### branches

we can add rules like, if perticuler branch trigger then only workflow exicute

```
    push:
    branches:
      - main # main
      - 'dev-*' # dev-new dev-this-is-new
      - 'fet/**' # fet/new fetnew/button
```


### Paths

if we were add path that means it will exicute if that path file have some cahnges

```
    paths:
      - '.github/workflows/*'
```

but when added `-ignore`, it simply ignore if there are some changes on that file

```
    paths-ignore:
      - '.github/workflows/*'
```

### fork

Understanding fork things, 


### skip

Simply added `[skip ci]` on commit message so that it will skip to exicute workflow.
