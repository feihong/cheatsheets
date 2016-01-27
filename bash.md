Find all files named .DS_Store:

```
find . -name '.DS_Store'
```

Find all files containing the string 'feihong', then replace occurrences of 'feihong.pythonanywhere' with 'chicktech.pythonanywhere'.

```
grep -rli 'feihong' * | xargs -i@ sed -i 's/feihong\.pythonanywhere/chicktech\.pythonanywhere/g' @
```
