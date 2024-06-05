# GitHub Actions Presentation

This is the sample app for GitHub Actions Presentation.

**WARNING: Please fork this repository and practice on your fork-repo.**

## Lab 1

There is an workflow located at `.github/workflows/hello-world.yaml`.

Let's add a new step into the Job named `hello`. It should execute the following command:

```bash
cat requirements.txt
```

## Lab 2

Now, let's create a new workflow `django.yaml` and perform Continuous Integration (CI) for the app.

1. Open your repository page in GitHub
2. Click on `Actions` tab
3. Click on `New workflow` button in the left column
4. Next, search workflow templates using keyword `Django`
5. In the search results, you will see the Django workflow template. Click on `Configure` button.
![image](https://github.com/devsuccess101/github-actions-bootcamp/assets/13513658/a2b4576a-a752-4615-a567-351d97d86884)
6. Now, set the python-version to v3.10:
```yaml
      matrix:
        python-version: ["3.10"]
```
7. Commit and make sure that the workflow is running

 ## Lab 3

 There is a `Dockerfile` file in this repository. It will be used to build the Docker image for this app.

 Let's create a new workflow for automate-building the Docker images in GitHub Actions and push them to GitHub Container Registry.
 
