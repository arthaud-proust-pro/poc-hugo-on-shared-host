# hugo-workflow-build
Template to build hugo and deploy it on a server by ssh 

# Setting up
Environment vars to set on github:
- HUGO_VERSION
- HUGO_ENV
- SSH_PRIVATE_KEY // server should have pair public key in its authorized_keys file
- SSH_USER
- SSH_HOST
- SSH_PORT
- SSH_WORKDIR // where builded files sould be copied


# How it works
Clone the repo and start to develop your website.  
Commit and push on the `develop` branch like any project.  
  
When you merge `develop` on production, github workflow will build and deploy on the server by ssh
