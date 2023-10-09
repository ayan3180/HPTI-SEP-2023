
 CONTRIBUTOR

                  ****** NETWORK PENTESTING TOOL ********
                                         
                        INTERN ID:- HPTI-SEP23-029
                              BY ANSHU ANAND
                        GITHUB USERNAME:- SAMAR911                
                          TOOL NAME:- ""NESSUS""

INTRODUCTION TO NESSUS

  Nessus is a vulnerability scanner that assists in finding and analyzing security flaws in a computer system. It identifies and prioritizes potential threats by utilizing a database of known vulnerabilities and exploits.

   Security experts rely on Nessus to perform vulnerability assessments, compliance audits, and malware detection. It is capable of scanning a wide range of devices, including servers, routers, firewalls, and virtual computers.

To use Nessus, you need to first install it on your system. Once installed, you can start it by running the Nessus start executable in Kali.
INSTALLATION

![1  nessus](https://github.com/gurusakharwade/HPTI-SEP-2023/assets/95374454/32c96106-7b46-4822-876d-232ef981dd3e)


Unlike many security tools, Nessus is not included with Kali Linux. However, it is quite simple to download and install. To install Nessus on your Kali, follow these steps:

  Download the Nessus package for Debian from the Nessus website https://www.tenable.com/downloads/nessus, making sure to select Linux-Debian-amd64 as the Platform.

Once the download is complete, open your Linux terminal and navigate to the directory where you saved the Nessus file.

Run the following command to install Nessus:

     dpkg -i Nessus-10.4.1-debian9_amd64.deb 

Start the Nessus service with this command:

     systemctl start nessusd

On your browser, go to https://kali:8834/. It would show a warning page

Click on Advanced. Then, click on Accept Risk and Continue.

Choose the Nessus Product you prefer. If you want the free version of Nessus, click on Nessus Essentials.

Enter your name and email address to receive an activation code by email. Paste the activation code into the space provided and choose a username and password.

Allow Nessus to download the necessary plugins.

HOW TO USE NESSUS

To initiate the Nessus service, run the following command in your terminal:

    systemctl start Nessus

Next, enter the following URL in your browser: https://kali:8834/

To access Nessus, you need to go to https://localhost:8834/# and log in using the username and password you set during installation.

    
After logging into Nessus, you can begin by creating a scan. In Nessus, there are other types of scans accessible, but let's start with a basic network scan. 

To create a new scan, click "New Scan" under the "Scans" tab. In the "New Scan" window, give the scan a name in the "Scan Name" area and 
provide the target domains or IP addresses in the "Targets" field. Multiple targets can be added by separating them with commas or spaces. 
We used Open Bug Bounty domains in this example.

Select "All ports" from the "Port scanning" dropdown menu under the "Discovery" section. This guarantees that all ports on the target systems are examined. 

Other options include configuring the maximum number of hosts to scan concurrently, the scan policy, and the credentials to use for authenticated scans. 

When you've finished configuring all of the options, click "Save" to save the scan setup.

Finally, press the "Launch" button to begin the scan. The scan may take some time to complete depending on the number of hosts and ports being examined.

The "Scans" tab allows you to track the scan's progress. When the scan is finished, click on the scan name on the "Scans" page to view the findings.  

The results will show you all of the vulnerabilities and issues discovered during the scan, as well as their severity level and recommended repair methods.

After customizing the scan, save it and run it like you would a standard network scan. The network vulnerability scan results will be shown in the same manner as the basic network scan results. Nessus will provide you with thorough information on any vulnerabilities discovered in the web application, as well as recommendations on how to resolve them.
    
  
