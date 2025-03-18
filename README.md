# spsh-app-deploy

This repository is used to automate deployments to the SPSH Devcluster.

# Deployments to the SPSH Devcluster

To automatically rollout and test a branch of any of this repository
- [dbildungs-iam-keycloak](https://github.com/dBildungsplattform/dbildungs-iam-keycloak)
- [schulportal-client](https://github.com/dBildungsplattform/schulportal-client)
- [dbildungs-iam-server](https://github.com/dBildungsplattform/dbildungs-iam-server)
- [dbildungs-iam-ldap](https://github.com/dBildungsplattform/dbildungs-iam-ldap)

one can use the Dev Pipeline. 

More info on what the Dev Pipeline does can be found on Confluence: [Dev Pipeline](https://docs.dbildungscloud.de/display/PROD/SPSH+Dev+Pipeline)

# Updating the Dev Pipeline 

If you have made changes on the Dev Piepline you need to create a new Release for the changes to become active. 
If you create a new major release the tag in these repositories has to get updated: 
- [dbildungs-iam-keycloak](https://github.com/dBildungsplattform/dbildungs-iam-keycloak)
- [schulportal-client](https://github.com/dBildungsplattform/schulportal-client)
- [dbildungs-iam-ldap](https://github.com/dBildungsplattform/dbildungs-iam-ldap)
- [dbildungs-iam-server](https://github.com/dBildungsplattform/dbildungs-iam-server)
- [spsh-app-deploy](https://github.com/dBildungsplattform/spsh-app-deploy/blob/main/.github/workflows/deploy.yml)

# Overwriting default Helm Chart values in Dev Piepline 
Via this repository the default values of the Helm Charts can get overwritten. See [SPSH Env Management]https://docs.dbildungscloud.de/display/PROD/SPSH+ENV+Management?src=contextnavpagetreemode for more information. 