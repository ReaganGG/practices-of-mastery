**Ansible: DevOps for IT Ops**

The following article is based on my experience as a middelware"IT Ops guys" and the benefits of Ansible.

**Background**
Ansible is different to other automation tools like Chef, Puppet and Salt. The main difference is that Ansible is first a push tool rather than a pull. In now way are the other tools mentioned inferior but Ansible offers an easier transision from no automation to fully automated.

**The Ansible awakening**
*Whats cool about Ansible?* Easy...you write stuff in YAML and Jinja2, which is so easy to learn my 3 year old daughter could write an Ansible playbook. You can do orcestraction from your laptop to your target servers without installing any additional software (As long as ssh and phython is installed).

*Whats bad about Ansible?* In my opinion...the documentation on the Ansible website. There docs are unecessarily complicated (for an IT Ops guy) especially some of the examples. But you quickly learn to "decrypt" it.

*What can Ansible do?* .....anything..... Well it cant make you carrot juice in the morning but you know what I mean. Any task that needs orcestration and automation.

*How does Ansible work?* By default it connects to your target machine via ssh (hopefully in your case using an ssh key that you have exchanged). It then runs your tasks that you have listed. Sounds easy but once you work through the concepts of roles, tasks, plays, playbooks and variables, you will realize that it is that simple.

*Will it work on Windows* Yes :(  (Im not a big windows fan)

*Why should Ansible be my entry into DevOps?* The Ansible path will quickly teach you how awesome it is to automate every repeatable task you have ever had. As an IT Ops guys I know that we love writing scripts and popping them into the crontab. If you want you can still have your scripts in a verion controlled repo which Ansible will deploy and add to the crontab for you.

One of the biggest questions I had when research Ansible was that, if it was so flexible and so cool why wasnt there an easy example of creating a playbook that diffreniated between all the test environments and production. After actually implementing Ansible I found the answer to the that question. Its because there is somemany many to this and so many different environment setup parameters. Because you can do this from your laptop there should be no reason why you shouldnt at least give this a try.