GitHub's `/?author=<foo>` differs from command-line Git's `--author=<foo>`.

This repository consists of a single commit, with username 'firstname1
lastname1' and email 'name1@example.com'.

If you limit the commits by the name 'name1', the Git CLI shows this
commit:

```
$ git log --oneline --author=name1
abc1234 Commit as name1
```

but using `--author` on GitHub does not:

https://github.com/pcharlan/commits-by-author/commits/master?author=name1

```
No commits found for "name1"
```

Giving the full email address instead of just the name portion will
list the commit on GitHub (and the CLI):

https://github.com/pcharlan/commits-by-author/commits/master?author=name1@example.com

This is command-line Git 2.6.2.
