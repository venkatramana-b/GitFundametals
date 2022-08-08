# GitFundametals
Automated ELK Stack Deployment
Automated ELK Stack Deployment

The files in this repository were used to configure the network depicted below.
(Add the Diagram here)


These files have been tested and used to generate a live ELK deployment on Azure. They can be used to either recreate the entire deployment pictured above. Alternatively, select portions of the ___yml and config__ file may be used to install only certain pieces of it, such as Filebeat. See in the Ansible folder for the below

•	Hosts
•	Ansible Configuration
•	Ansible ELK Installation and VM Configuration
•	Filebeat Config
•	Filebeat Playbook
•	Metricbeat Config
•	Metricbeat Playbook
 

This document contains the following details:
-	Description of the Topology
-	Access Policies
-	ELK Configuration
-	Beats in Use
-	Machines Being Monitored
-	How to Use the Ansible Build


Description of the Topology

The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.
Load balancing ensures that the application will be highly __functional and available___, in addition to restricting __traffic___ to the network.

What aspect of security do load balancers protect?
The Load balancers add resiliency by rerouting live traffic from one server to another if a server falls prey to a DDoS attack or otherwise becomes unavailable.

What is the advent age of a jump box?
A Jump Box Provisioner is also important as it prevents Azure VMs from being exposed via a public IP Address. This allows us to do monitoring and logging on a single box. We can also restrict the IP addresses able to communicate with the Jump Box, as we've done here

Integrating an ELK server allows users to easily monitor the vulnerable
VMs for changes to the __network___ and system __logs___.

What does Filebeat watch for?_
Filebeat monitors the log files or locations that you specify, collects log events, and forwards them either to Elasticsearch or Logstash for indexing

What does Metricbeat record?_
Metricbeat takes the metrics and statistics that it collects and ships them to the output that you specify, such as Elasticsearch or Logstash.

