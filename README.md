# n8n-gitlab
poc of n8n workflows with non-internet gitlab instance


## Deploy Gitlab Azure vm
https://docs.gitlab.com/ee/install/azure/


## Deploy n8n Azure vm
1. Deploy Azure Unbuntu 20.04 VM, Standard D4s v3 (4 vcpus, 16 GiB memory)
1. ssh to vm using private key provided (copy to %USERPROFILE%\.ssh)
1. Install node.js version manager:
   - `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash`
   - restart ssh session
   - run `command -v nvm` to verify installed (expect nvm command to be listed)
1. Install latest version of node.js
   - `nvm install node`
1. Install n8n npm package (globally)
   - `npm install n8n -g`
1. start n8n
   - `n8n start`