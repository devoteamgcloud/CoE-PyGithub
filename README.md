# PyGitHub

Fprked PyGithub for CoE
PyGitHub is a Python library to access the [GitHub REST API].
This library enables you to manage [GitHub] resources such as repositories, user profiles, and organizations in your Python applications.

[GitHub REST API]: https://docs.github.com/en/rest
[GitHub]: https://github.com

## Install

```bash
$ pip install PyGithub
```

## Simple Demo

```python
from github import Github

# First create a Github instance:

# using an access token
g = Github("access_token")

# Github Enterprise with custom hostname
g = Github(base_url="https://{hostname}/api/v3", login_or_token="access_token")

# Then play with your Github objects:
for repo in g.get_user().get_repos():
    print(repo.name)
```

## Documentation

More information can be found on the [PyGitHub documentation site.](https://pygithub.readthedocs.io/en/latest/introduction.html)

