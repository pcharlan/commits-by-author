GitHub's `/?author=<foo>` differs from command-line Git's `--author=<foo>`.

This repository consists of a single commit, with username 'firstname1
lastname1' and email 'name1@example.com'.

Limiting commits by the name 'name1' will show this commit on the Git command-line, but not using the GitHub interface for limiting commits by author:

```
$ git log --oneline --author=name1
abc1234 Commit as name1
```

When listing commits via GitHub:

https://github.com/pcharlan/commits-by-author/commits/master?author=name1

The output is:

```
No commits found for "name1"
```

Giving the full email address works:

https://github.com/pcharlan/commits-by-author/commits/master?author=name1@example.com

This is command-line Git 2.6.2.
