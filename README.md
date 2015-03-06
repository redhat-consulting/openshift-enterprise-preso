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
