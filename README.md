## Chart dependency update

`helm dependency update`

## Chart package
```bash
$ helm package jira # build the tgz file and copy it here
```

## Repo index
```bash
$ helm repo index . # create or update the index.yaml for repo
```

# How to use it as a helm repo

You might know github has a raw view. So simply use the following:

```bash
$ helm repo add raimangsxr 'https://raw.githubusercontent.com/raimangsxr/charts'
$ helm repo update
$ helm search jira
```

If your repo is private you can create a "Personal access tokens" and use it like:

```bash
$ helm repo add raimangsxr 'https://MY_PRIVATE_TOKEN@raw.githubusercontent.com/raimangsxr/charts'
```
