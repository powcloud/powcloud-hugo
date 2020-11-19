# PowCloud Hugo

## Install

1. Make your site a module itself
```hugo mod init <github.com/repo/project>```

2. Add this module you want to import to your config.toml:
```
[[module.imports]]
    path="github.com/drush/powcloud-hugo"
    disable=false
```

3. Run hugo

```
hugo server
```

At this point, the remote module will be downloaded and overlayed onto your own project and any resources will be available to your project.

## Upgrade All Modules to Latest
```
hugo mod get -u ./...
```

