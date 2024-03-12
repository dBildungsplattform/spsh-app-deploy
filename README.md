# spsh-app-deploy

This repository is used to automate deployments to the SPSH Devcuster and to manage rollout to the SPSH Staging and Prod Cluster.  

# Deployments to the SPSH Devcenter 

To automatically rollout and test a branch of any of this repository
- [dbildungs-iam-keycloak](https://github.com/dBildungsplattform/dbildungs-iam-keycloak)
- [schulportal-client](https://github.com/dBildungsplattform/schulportal-client)
- [dbildungs-iam-server](https://github.com/dBildungsplattform/dbildungs-iam-server)

one can use the Dev Pipeline. 

More info on what the Dev Pipeline does can be found on Confluence: [Dev Pipeline](https://docs.dbildungscloud.de/display/PROD/SPSH+Dev+Pipeline)



# Rollouts to the Staging and Prod Instance 

Also the Rollouts ......

For more information on the Release Process, see this Confluence Page: [Dev Pipeline](https://docs.dbildungscloud.de/display/PROD/SPSH+Releasemanagement)



# Debugging the Release Proces 
 to debug the release process change the ref of the code that is checked out in the rollout-release.yml repository. Yuo can also trigger a releae via github cli ("gh") by running this command. 
 ```
gh workflow run rollout-to-instance.yml -f release_tag="release-tag" -f target_instances="target_instance" --ref branch_name
```