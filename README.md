# ABOUT

Simple Vue app to display my own portfolio.

The purpose of this is for others to also show off their own portfolio by forking this and using it as a template.

This is utilizing Github Pages to show off a free website.

Thanks to Github for providing this free for all of their users!

# SETUP

## Requirements and installation

Update your Node/npm version to at least:
```bash
`Node.js v18.12.1`

`npm@9.2.0`
```
Node/npm can be installed from [nodejs.org](https://nodejs.org)

Install and update Vue to at least:
`@vue/cli 5.0.8`

```bash
`npm install -g @vue/cli`
```

## Serving locally

```bash
cd ./src
npm run serve
```

# Contributing/Making it your own

Make sure you are familiar with vue.
But if you aren't, don't fear, most of this repository will be kept very simple.

## Steps:

### Fork the repo

After you fork the repo, clone it down locally:
```bash
example:
git clone https://github.com/rory-wagner/portfolio
```

### Run the project locally

After running through the SETUP section above:

```bash
cd ./src
npm run serve
```

### Make sure your github pages are updating

This has not been tested to work on forked repos (as I don't own them).
However, you might want to check and see if they are working by following this [guide](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages).
Make sure that the workflow inside of ```.github/workflows/main.yml``` is fixed for your repo.
Now go have fun with it!
