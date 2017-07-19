PEP8 Git Commit Hook
====================

This is a pre-commit hook for Git that checks the code to be committed
for Python PEP8 style compliance.  The hook will prevent the commit in
case style violations are detected.

Installation:

1. Install the pycodestyle (formally called pep8) program: ```$ pip install pycodestyle```
2. Save pre-commit as your_project/.git/hooks/pre-commit
3. Mark pre-commit executable: ```$ chmod +x your_project/.git/hooks/pre-commit```

The hook can be overridden: ```$ git commit --no-verify```

In case you want to modify the list of codes to ignore, edit the
```ignore_codes``` list in the pre-commit file.   
If you want to select only specific codes to scan for, use the
```select_codes``` list.
Additional arguments to the pycodestyle program (e.g., ```--max-line-length=120```) can be added to the ```overrides``` list.

This code was forked from [https://gist.github.com/810399](https://gist.github.com/810399).
