# Heimdall Website

## Setup development environment
This setup assumes you have Hugo installed

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