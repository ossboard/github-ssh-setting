
### 설정방법

```
$ ssh-keygen -t rsa -C "ossboard@gmail.com"
  엔터,엔터,엔터
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/id_rsa
$ pbcopy < ~/.ssh/id_rsa.pub  <--클립보드복사

https://github.com/settings/keys
( 설정>Access>SSH and GPG keys )
SSH keys > 'New SSH key' > title:macbook , Key:key 붙여넣기

$ ssh -T git@github.com
Hi ossboard! You've successfully authenticated, but GitHub does not provide shell access.


이후부터, 해당 PC에서는 SSH 로 clone,push 등 하면 패스워드 없이 가능함!

```
