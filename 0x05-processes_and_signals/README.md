#!/bin/bash
git add .
echo "enter commit title: "
read commit_title
git commit -m "$commit_title"
result=$?
if [ $result -eq 0 ]; then
        git push
else
        echo "commit failed"
fi
~
