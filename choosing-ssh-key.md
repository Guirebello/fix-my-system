In order to choose wich key you are going to use for gitlab and github for example, you can do the following:

## Create config file
in your `.ssh/` folder:
```shell
touch config
```
## Edit the config file
them, in your editor of preference, open config and write the following:
```
# GitHub configuration
Host github.com 
	HostName github.com 
	User git 
	IdentityFile ~/.ssh/id_rsa_github 

# GitLab configuration 
	Host gitlab.com 
	HostName gitlab.com 
	User git 
	IdentityFile ~/.ssh/id_rsa_gitlab
```
in the `IdentifyFile` field, you should put the name of the ssh key file you want to use for the given host