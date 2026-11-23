создать .md

1. установить python-pymupdf4llm из AUR
$ pamac build python-pymupdf4llm

2. выполнить команду. она создаст md-файл в той же папке, что в pdf-файл.
$ python -c "import pymupdf4llm; md = pymupdf4llm.to_markdown(<ИМЯ_ДОКУМЕНТА>.pdf'); open('<ИМЯ_ДОКУМЕНТА>.md', 'w', encoding='utf-8').write(md)"
