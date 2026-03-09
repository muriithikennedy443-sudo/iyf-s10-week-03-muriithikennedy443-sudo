Task 5.2 challenge: Portfolio Reorganisation
Final project structure:
.
./docs
./tests
./src
./src/css
./src/images
./src/js
All foles in project:
./docs/README.md
./docs/backup.html
./terminal-log.md
./README.md
./src/css/style.css
./src/js/main.js
Q1: HTML files in my project:
./docs/backup.html
Q1: HTML files in my project:
./docs/backup.html
./contact.html
./index.html
./about.html
Q2: Files containing contact:
Q3: CSS file line count:
0 src/css/style.css
Q4: My last 10 terminal commands:
   64  grep -r "contact" . >> terminal-log.md
   65  grep -r "contact" . --exclude="terminal-log.md"
   66  grep -r "contact" . --include="*.html"
   67  grep "contact" contact.html >> terminal-log.md
   68  ls src/css
   69  wc -l src/css/style.css
   70  echo "Q3: CSS file line count:" >> terminal-log.md
   71  wc -l src/css/style.css >> terminal-log.md
   72  history | tail -10
   73  history | tail -10 >> terminal-log.md
Task 5.4: Shell Basics
Script contents:
#!/bin/bash
# Create a new project withstandard structure

PROJECT_NAME=$1

if [ -z "PROJECT_NAME" ]; then
   echo "Usage: ./new-project.sh project name"
   exit 1
fi

mkdir -p "$PROJECT_NAME"/{src/{css,js,images},docs,tests}
touch "PROJECT_NAME"/README.md
touch "PROJECT_NAME"/src/index.html
touch "PROJECT_NAME"/src/css/style.css
touch "PROJECT_NAME"/src/js/main.js

echo "# $PROJECT_NAME" > "$PROJECT_NAME"/README.md
echo "Project $PROJECT_NAME created successfully!"
Script test result - project structure created:
my-awesome-app
my-awesome-app/docs
my-awesome-app/tests
my-awesome-app/src
my-awesome-app/src/css
my-awesome-app/src/images
my-awesome-app/src/js
Task 6.2: Branching and Merging
Commit history after all exercises:
47d8991 fix: resolve merge conflict in index.html
e2565fe feat: add heading version B
1052327 feat: add heading version A
eab8ac7 feat: add about page content
3f004d2 docs: update README with project information
acb7b26 fix: correct responsive breakpoints
d20276b feat: add navigation styling
0643108 Completed Task 5.4 shell script basics
bbc8e17 Complete Task 5.3 useful terminal commands
2724d80 Added index.html, contact.html, and about.html to terminal-practice
a498c5f Completed Task5.2 reorganisation challenge
cebbc2b Merge branch 'main' of https://github.com/muriithikennedy443-sudo/iyf-s10-week-03-muriithikennedy443-sudo
07e54f6 Completed Task 5.2 file operation
6e9c9ca Add .gitkeep to keep empty folders
44afc17 Update terminal-log.md with HTML line breaks
b780887 Add terminal-log.md
c215fd9 Initial commit
Current branches:
  feature/contact-form
  feature/new-header
* main
