git init && git add . && git commit -m "first commit" && git branch -M master && git remote add origin https://github.com/hwalanlee/ansible-test.git && git push -u origin master
git add . && git commit -m "commit" && git push -u origin master

https://github.com/panduroab/ansible-nodejs-playbook/blob/master/main.yml
------------------------------------------------------------------------------

- ansible 설치 > inventory(/etc/ansible/hosts) 설정 > known hosts 등록 > 신규 inventory 설정

- 키페어 지정
    - /etc/ansible/ansible.cfg
        - private_key_file = /home/ec2-user/lanKeyPair.pem

--------------------------------------------------------
- gateway server
    - /etc/ansible/hosts - hosts

- remote server


--------------------------------------------------------
- ansible all -m ping
    - known hosts 등록

-------------------------------------------------------------

시나리오
- README.md
- hosts
- main.yml
- start.sh
- tasks
    - git-install.yml
    - nodejs-install.yml
    - web-clone.yml
    - web-start.yml
