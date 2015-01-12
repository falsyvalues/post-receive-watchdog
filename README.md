# post-receive-watchdog
Git post-receive hook for tracking changes about which you would like to know

This tool helps track file changes (only*) in certain files in your git repository.

Configuration is dead simple, its based on ini file and python <a href="https://docs.python.org/2/library/re.html">regular expression</a> for file matching:

# config example:

```
[AllChanges]
recipients:
    info@example.com
files:
    .*

[OtherGroup]
recipients:
    other@example.com
files:
    single-file.py
```

# future features

* tracking on specyfic branch
* tracking operations on branches / tags (create, delete)


<a href="https://www.bentasker.co.uk/documentation/development-programming/288-sending-commit-notifications-on-receive-using-git-post-hooks">Ben Tasker</a> post-receive hook
<a href="https://github.com/git/git/blob/master/contrib/hooks/post-receive-email">original post-receive-email hook</a>

Thanks to @stachjankowski for help.
