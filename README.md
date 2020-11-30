add IP addresses to the local inventory file ./hosts like this:
[build]
build1 ansible_host=10.129.0.18
[prod]
prod1 ansible_host=10.129.0.32

Executing ansible-playbook:
ansible-playbook -i ./hosts -v test-serv.yml

See the result on the WEB:
http://<IP>:8080/hello-1.0/