# post-receive-watchdog
Git post-receive hook for tracking changes about which you would like to know

This tool helps track file changes (only*) in certain files in your git repository.

Configuration is dead simple, its based on ini file and python [regular expression](https://docs.python.org/2/library/re.html) for file matching:

## config example:

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

## features under development

* tracking on specyfic branch
* tracking operations on branches / tags (create, delete)
* move some configuration to git

## helpful links

* [Ben Tasker post-receive hook](https://www.bentasker.co.uk/documentation/development-programming/288-sending-commit-notifications-on-receive-using-git-post-hooks)
* [Original post-receive-email hook](https://github.com/git/git/blob/master/contrib/hooks/post-receive-email)

## Others
Thanks to [@stachjankowski](https://github.com/stachjankowski) for help.
