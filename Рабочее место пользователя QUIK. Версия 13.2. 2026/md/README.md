**Как создать Markdown-документ из PDF-документа**

1. Установить `python-pymupdf4llm` из **AUR**
```
$ pamac build python-pymupdf4llm
```

2. Выполнить команду. Она создаст файл `doc.md` в той же папке, что в `doc.pdf`.
```
$ python -c "import pymupdf4llm; md = pymupdf4llm.to_markdown('doc.pdf'); open('doc.md', 'w', encoding='utf-8').write(md)"
```
