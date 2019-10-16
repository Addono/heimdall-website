# Heimdall Website
This is the source code of Heimdall's website, see it live at [https://heimdall.ga](https://heimdall.ga).

## Development
This website is build using the statis site generator [Hugo](https://gohugo.io/), please refer to their excellent "[Getting started](https://gohugo.io/getting-started/usage/)" documentation.

### Setup
This setup assumes you have Hugo installed. If not, it's easy, found out [here](https://gohugo.io/getting-started/installing/) how for your platform.

```sh
# Clone the website repo:
git clone --recurse-submodules https://gitlab.com/heimdall-surveillance/heimdall-surveillance.gitlab.io.git

# Start a local server
cd heimdall-surveillance.gitlab.io
hugo server
```

If you also want to work on the theme then make sure that the `HEAD` is on one of the branches, e.g. when working on `master`:
```sh
cd themes/hugo-icon
git checkout master
cd ../../
```

## Contributing

[CI/CD](https://gitlab.com/heimdall-surveillance/heimdall-surveillance.gitlab.io/pipelines) is setup to automatically build every commit. In addition, the `master`-branch automatically deploys. For this reason, `master` is protected such that only users with the "maintainer" status can push or merge code into the production environment. 

Don't let this fool you, merge requests are always welcome! Just make an MR and assign one of the maintainer. When in doubt, use @addono.