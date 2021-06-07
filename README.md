# ocp4_rbac
This Ansible role allows OCP4 cluster admins to create and manage cluster roles and project roles by choosing which type of role and action they want to implement.  Instead of inputting the command for each, just go to the defaults/main.yml and define the variables for what you'd like done and run the playbook.

### Cluster Roles
The cluster_role.yml has tasks to create a cluster role, and add/remove it from users/groups.  If you don't need to create a cluster role and just want to add/remove one of the 8 default cluster roles, simply define the cluster_role_name with one of those and choose not to create a cluster role.


### Project Roles
The project_role.yml has tasks to create a project role, and add/remove it from users/groups.  If there is an existing role that can be used for your project, define the role_name with that existing role and choose not to create a new project role.  You can also add an SCC to a service account for your project with this playbook.  
