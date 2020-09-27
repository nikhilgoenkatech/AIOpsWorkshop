DISCLAIMER: This project was developed for educational purposes only and is not complete, nor supported. It's publishment is only intended for helping others automate environments for delivering workshops with Dynatrace.

Inspired/Borrowed from similar package by Sergio Hinojosa.

# AIOpsWorkshop
The script to install all the pre-requisites in order to run a hands-on session for AIOps.

A simple Bash script will set-up a fully functional Single Node Dynatrace installed and required dockers installed. This script can be used to run the commands on a LINUX/UBUNTU Server 18.04 LTS & 20.04 LTS.

Features in a Nutshell
-----------------------
Update the ubuntu repository
Installation of Docker (for building own Docker images)
Installation of Microkubernetes
Set up of useful BASH Aliases for working with the command line
Installation of Dynatrace ActiveGate and configuration of Cluster and Workload monitoring
Enabling own Docker Registry for the Cluster
Installation of Dynatrace OneAgent.
Create a user account and copy the standard user (ubuntu on this case) with his own home directory (a replica) and allowing SSH connections with text password. Useful for spinning an army of workshop clusters.
Download apache-jmeter which can be used in order to showcase Jenkins/Dynatrace integration.
Download proprietary Jenkins docker image created for such workshop.
Dpwnload proprietary Sample Bank Application Docker created for bank organizations.
Download standard ansible-tower which could be used for workshop.
Download the Dockerfile/repositories required to run the workshops.

More about the script:
Script has boolean flags which can act as control flags in order to enable/disable the features. Currently, the available features would have multiple dockers installed, however,going forward more features can be added - for example, micro-k8s can be added to control and spin these dockers or a keptn on top of k8s. The repository mainly contains the following file:
install-workshop-tech-stack.sh
install-prerequisites.sh

Run the script:
Run it in an available machine (manually)
1. Log in into your Ubuntu image
2. Clone the repo and navigate to the directory
git clone AIOPsWorkshop ; cd AIOPsWorkshop

3. Execute the file with sudo rights.
sudo bash -c './install-workshop-tech-stack.sh &'

For inspecting the installation on realtime type:
less +F /tmp/install.log


