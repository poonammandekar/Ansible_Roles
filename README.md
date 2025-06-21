1.site.yaml is the master file to deploy war on host1 using ansible playbook.

2.deploy_docker.yaml is the master file to deploy war on host2 using docker.

3.the roles folder contains roles defines for  deploy war on host1 

4.roles/tomcat_deploy contains tasks ,vars,handlers defined to  deploy war on host1 

5.roles/docker_build_run contains tasks, var, files to deploy war on host2 using docker.
