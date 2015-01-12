## post-receive-watchdog
Git post-receive hook for tracking (email notifications) changes which you would like to know about.

This tool helps to track changes in certain files (only*) in your git repository.

Configuration is dead simple. It's based on ini file and python [regular expression](https://docs.python.org/2/library/re.html) for file matching:

### config example:

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

### features under development

* tracking on specyfic branch
* tracking operations on branches / tags (create, delete)
* moving some of configuration to git

### helpful links

* [Ben Tasker post-receive hook](https://www.bentasker.co.uk/documentation/development-programming/288-sending-commit-notifications-on-receive-using-git-post-hooks)
* [Original post-receive-email hook](https://github.com/git/git/blob/master/contrib/hooks/post-receive-email)

### others
Thanks to [@stachjankowski](https://github.com/stachjankowski) for help.