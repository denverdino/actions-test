# actions-test

Test project for some github actions

1. ACR login: https://github.com/denverdino/acr-login
2. ACR scan: https://github.com/denverdino/acr-scan


## Local test

```
act -P ubuntu-latest=denverdino/act-base --secret-file my.secrets
```

Note:

If you hit the problem with ```Error response from daemon: experimental session with v1 builder is no longer supported, use builder version v2 (BuildKit) instead```, please add 

```"features": { "buildkit": true }``` to ``` /etc/docker/daemon.json```  as a workaround

