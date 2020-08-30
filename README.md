# DOF Exam 2019.02.10 / 2019.02.17 / 2019.04.07 / 2020.08.30
Exam Repository for DevOps Fundamentals Course @ SoftUni

A set of three Docker containters each with a dedicated role - *php*, *redis*, and *nginx*, that form a simple web application.

For a successful completion you have to:
 - (re)build the images;
 - (re)push the images;
 - (re)run the containers;
 - (re)apply the changes on the running application;

Please note that when modifying the solution for platform of your choice (k8s or nomad) changes must be made:
 - the **app** folder must be copied where (in terms of path and images) applicable;
 - **Dockerfile** files must be updated where applicable;
 
General application notes:
 - php files are expected to be in the **/site** folder of both the *nginx* and *php* containers;
 - each container should be named after the following rule - **role-host**, where *role* is *php*, *redis*, or *nginx*. For example, **php-host**;
 - mind the ports - each container is listening on a specific port, for example *nginx* is set to listen on port **80**;
 - *nginx* container should be started after *php*;

Use the **docker-compose.yml** file as a starting point when building the final set of application configuration files for the platform of your choice. You can use a tool to build and then modify them, or do the entire process manually. 
