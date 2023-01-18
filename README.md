Default Community health files for Consenlabs
projects. such aspull request template, issue template, etc...

# Copy pll request template file to your repo

In the root of the repository call those scripts,
you can change your file target if your pull request template file not under `.github` folder

```
curl -o target/path/filename URL
```

## Backend

```
curl -o .github/PULL_REQUEST_TEMPLATE.md https://raw.githubusercontent.com/consenlabs/github-health-file-template/main/docs/PULL_REQUEST_TEMPLATE/be-pull-request-template.md
```

## Frontend

```
curl -o .github/PULL_REQUEST_TEMPLATE.md https://raw.githubusercontent.com/consenlabs/github-health-file-template/main/docs/PULL_REQUEST_TEMPLATE/fe-pull-request-template.md
```
