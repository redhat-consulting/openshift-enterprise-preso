# Red Hat Slide Template for Reveal.js

## Installation Options

### Install Locally

1. Install Node & NPM
2. Clone Repo
```bash
git clone git@github.com:redhat-consulting/slide-template.git
```
3. Navigate to root project
```bash
cd slide-template
```
3. Install Dependencies
```bash
npm install
```
4. Run server
```bash
npm start
```
5. Open browser and navigate to: http://127.0.0.1:8000

### Run in OpenShift

```bash
rhc app create slidetest nodejs-0.10 --from-url git@github.com:redhat-consulting/slide-template.git
```

## Creating Decks

To create a new slide deck, simply copy this one. Here are some steps to do this responsibly using git.

1. Greate a local git repo
```bash
mkdir my-new-slides
cd my-new-slides
git init
```

2. Add this repo as an upstream project so you can pull in template updates
```bash
git remote add upstream git@github.com:redhat-consulting/slide-template.git
```

3. Pull initial content from github
```bash
git pull upstream master
```

4. Write Your Content

The content for your slides is all contained in slides.md. Use [Githib Flavored Markdown](https://help.github.com/articles/github-flavored-markdown/) to create your slides.
