…or create a new repository on the command line if only u want to push new changes
echo "# Books" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/NavalKishor/Books.git
git push -u origin master

…or push an existing repository from the command line if only u want to push new changes
git remote add origin https://github.com/NavalKishor/Books.git
git push -u origin master

Create a new repository if only u want to get a copy and push new changes
git clone https://gitlab.com/navalgitlab/books.git
cd books
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

Existing folder if only u want to push new changes
cd existing_folder
git init
git remote add origin https://gitlab.com/navalgitlab/books.git
git add .
git commit -m "Initial commit"
git push -u origin master

Existing Git repository if only u want to push new changes
cd existing_repo
git remote rename origin old-origin
git remote add origin https://gitlab.com/navalgitlab/books.git
git push -u origin --all
git push -u origin --tags
