# hugo-workflow-build
Template to build hugo with github workflows on a build branch

# How it works
Clone the repo and start to develop your website.  
Commit and push on the `develop` branch like any project.  
  
Github workflow will build hugo site when you commit/merge on deploy branches. Then, workflow will push builded site on the right branch:  
- `validation` => `build-validation`
- `production` => `build-production`
