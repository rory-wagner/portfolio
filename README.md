# ABOUT

Simple Vue app to display my own portfolio.
This is open source.
Anyone is allowed to copy this for their own portfolio or fork and use it as a template.

# SETUP

## Requirements and installation

`Node.js v18.12.1`
`npm@9.2.0`

Node/npm can be installed from nodejs.org

`@vue/cli 5.0.8`

`npm install -g @vue/cli`

## Serving locally

`cd` into `./src`

`npm run serve`

## Serving in Github Pages

[Home Page](https://rory-wagner.github.io/portfolio/)

# Contributing/Making it your own

Make sure you are familiar with vue.
But if you aren't, most of this repo will be kept very simple.

## Steps:

### Clone the repo

```bash
example clone:
git clone https://github.com/rory-wagner/portfolio
```

### Run the project locally

After getting npm installed:

```bash
cd ./portfolio
npm run serve
```

### Make sure your github pages are updating

This has not been tested to work on forked repos (as I don't own them).
However, you might want to check and see if they are working by following this [guide](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages).
Make sure that the workflow inside of ```.github/workflows/main.yml``` is fixed for your repo.
