# Generate Key
```shell
ssh-keygen -t ed25519 -C "<comment>"
```
- For Github and Gitlab
	- inside "" you can enter the email of your account

## Getting the key
you can `cat` the **.pub** key file in the `.ssh/` folder and use it in Github or Gitlab for example


Reference: https://docs.gitlab.com/user/ssh/