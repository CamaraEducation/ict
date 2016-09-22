# ICT Documentation

### How to contribute to this project

1. Taken from http://docs.readthedocs.io/en/latest/getting_started.html

    $ pip install sphinx sphinx-autobuild

2. To auto update as you write your document. The _build_html/index.html will be updated every time you update your document:

    $ sphinx-autobuild . _build_html

3. To build the output (folder `_build`):

    $ make html

### How to add new documents

1. All the documents are stored in docs/ folder.
2. Create a folder for your documentation and then link it on index.rst
3. There's a script called docx2md.sh that you can use to convert docx files to markdown.

### Deployment for RACHEL

1. Run `make html` to update the _build folder. It will get picked up by rachel-index.php automatically
2. On the client, update by getting the file: `wget --no-check-certificate https://github.com/SystemR/ict/archive/master.zip`
3. If the repository was checked out using git, do a `git pull` on the folder to update

### Deployment for Read The Docs

1. Every time you commit and push to the git repo, http://ict.readthedocs.io/ will be updated with the latest documentation