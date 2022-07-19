# hugo-workflow-build
Template to build hugo with github workflows on a build branch

# Setting up
Environment vars to set on github:
- HUGO_VERSION
- HUGO_ENV
- SSH_PRIVATE_KEY // should be the private key of your server?
- SSH_USER
- SSH_HOST
- SSH_POST
- SSH_WORKDIR


# How it works
Clone the repo and start to develop your website.  
Commit and push on the `develop` branch like any project.  
  
When you merge `develop` on production, github workflow will build and deploy on the server by ssh
