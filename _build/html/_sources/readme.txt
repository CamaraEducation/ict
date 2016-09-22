# ICT Documentation

## How to contribute to this project

1.

## How to add new documents

1. All the documents are stored in docs/ folder.
2. Create a folder for your documentation and then link it on index.rst
3. There's a script called docx2md.sh that you can use to convert docx files to markdown.

## Deployment for RACHEL

1. Run `make html` to update the _build folder. It will get picked up by rachel-index.php automatically
2. On the client, update by getting the file: `wget --no-check-certificate https://github.com/SystemR/ict/archive/master.zip`
3. If the repository was checked out using git then do a `git pull` on the folder to update
