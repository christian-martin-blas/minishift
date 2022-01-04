# minishift
Repository with instructions for testing Minishift

## Openshift CLI configuration
```
$ minishift oc-env
export PATH="/home/john/.minishift/cache/oc/v1.5.0:$PATH"`
# Run this command to configure your shell:
# eval $(minishift oc-env)
```

## Basic minishift commands
### Start minishift
`minishift start`

### Start minishift with proxy configuration

```
 minishift start --http-proxy http://<proxy_username>:<proxy_password>@YOURPROXY:PORT --https-proxy https://<proxy_username>:<proxy_password>@YOURPROXY:PORT
```

### Stop minishift
`minishift stop`

### Status minishift
`minishift status`

### Default minishift user/password
`developer/developer`

## First openshift commands

### Change context to default
``oc config use-context current``

### Login in openshift
``oc login https://172.28.128.184:8443/ -u developer``

### Openshift Web Console
`https://172.28.128.184:8443/`