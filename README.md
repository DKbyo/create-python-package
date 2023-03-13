# create-python-package

After [connected your Github repository](https://cloud.google.com/build/docs/automating-builds/github/connect-repo-github), you could create your own trigger for every branch that starts with v.

```
gcloud beta builds triggers create github \
--repo-name="YOUR_GITHUB_REPO_NAME" \
--repo-owner="YOUR_GITHUB_USER" \
--tag-pattern=v \
--substitutions _REPOSITORY=https://REGION-python.pkg.dev/YOUR_PROJECT/YOUR_AR_REPO_NAME \
--build-config=cloudbuild.yaml
```

For more information about this, please visit.

[https://cloud.google.com/build/docs/building/build-python](https://cloud.google.com/build/docs/building/build-python)
