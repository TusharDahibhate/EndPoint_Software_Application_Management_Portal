# Endpoint Software/Application Management Portal

This project served as the final year project for the partial fulfilment of my Bachelor's degree in Computer Engineering from 
Singhad College of Engineering(Pune University). This project was completed by a team of 4 under the guidance of Prof. A.R. Joshi along 
with seasoned mentors from the industry.

The repository contains the resources relevant to the project.

## Description
The installation of any software requires prior knowledge of the software dependencies which only a person with some technical background 
will have. The installation process could be tedious and time consuming at times. This project will manage software and applications on 
any endpoint. It will be used to automate the process of software installation to reduce the manual efforts required during installation 
of a software. It will also be used to provide application execution environments. 

## Automation of software installation using Chef:

<img src="https://github.com/TusharDahibhate/EndPoint_Software_Application_Management_Portal/blob/master/images/chef.png" width="600">

### Intuition:
1. The application server will also serve as the Chef Server and Chef Workstation.
2. The UI will accept the IP address and credentials of the endpoint on which we need the software to be installed.
3. Chef server will accept this data and initiate bootstrapping of the endpoint(If it is not already bootstrapped).
4. Chef server will then upload the appropriate cookbooks as per the software selected, onto the endpoint. 
5. The client will then execute the cookbooks, thus installing the software.

## Provision of execution environment using Docker:

<img src="https://github.com/TusharDahibhate/EndPoint_Software_Application_Management_Portal/blob/master/images/docker.png" width="600">

### Intuition
1. The endpoints have docker installed on them. 
2. The UI will accept the desired IP address, credentials, execution environment and the necessary web application code to execute. 
3. The server will secure copy the contents and initiate a docker build on the endpoints using the Docker remote API. 
4. The server will then spawn the containers once the build is done and the code will be placed in the environment. 
5. Overall, we packaged the application and all the dependencies needed for that application to execute in isolated containers in a platform independent manner.


## Tech Stack
* Backend
    * Java 
    * Java Servlets
* FrontEnd
    * HTML
    * CSS
    * Bootstrap
* Tools
    * Chef
    * Docker
    * Eclipse
    

## Resources

[Synopsis](https://github.com/TusharDahibhate/EndPoint_Software_Application_Management_Portal/blob/master/reports/synopsis.pdf)

[Final Report](https://github.com/TusharDahibhate/EndPoint_Software_Application_Management_Portal/blob/master/reports/Final_Report/thesis.pdf)

[Publication](https://github.com/TusharDahibhate/EndPoint_Software_Application_Management_Portal/blob/master/reports/Publication/Paper.pdf)

[Presentation](https://github.com/TusharDahibhate/EndPoint_Software_Application_Management_Portal/blob/master/reports/Review_presentation.pdf)
