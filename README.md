# Gidpod workspace template
Template of my gitpod workspace.  
Use confidential information using [HashiCorp Vault](https://www.vaultproject.io/).  
Vault is S3 Storage Backend.  
When using, the following environment variables must be set.  

# Environment Variables
|  Name  |  Explanation of value   |
| ---- | ---- |
|  VAULT_A_KEY  |  AWS_ACCESS_KEY_ID used for S3 access  |
|  VAULT_S_KEY  |  AWS_SECRET_ACCESS_KEY used for S3 access  |
|  VAULT_BUCKET  |  S3 bucket name to store Vault  |
|  VAULT_REGION  |  S3 bucket region  |
|  VAULT_UNSEAL_KEY  |  Key to unseal Vault  |
|  VAULT_TOKEN  |  Token for login to Vault  |

# Base image
[gitpod/workspace-full:latest](https://hub.docker.com/r/gitpod/workspace-full)

# Installed applications
- [anyenv](https://github.com/anyenv/anyenv) and [anyenv-update](https://github.com/znz/anyenv-update)
- [AWS CLI version 2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-linux.html)
- [git-secrets](https://github.com/awslabs/git-secrets.git)
- [HashiCorp Vault](https://www.vaultproject.io/)
- [kr](https://krypt.co/docs/start/installation.html)
- [tig](https://jonas.github.io/tig/)
- [tmux](https://github.com/tmux/tmux)
