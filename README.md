# mgjeon.github.io

## Quickstart

Clone this repository
```
git clone https://github.com/mgjeon/mgjeon.github.io
cd mgjeon.github.io
```

Check blog in local
```
quarto preview
```

Remove metadata of ipynb files
```
nbdev_clean --fname posts/
```

Update main branch
```
git add .
git commit -m "update"
git push
```

Publish the changes
```
quarto publish gh-pages
```