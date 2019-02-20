# Threat Analysis and Server Lockdown
The goal of this project was to understand what an *insecure* operating system looked like, to assess it and to lock it down. This included the below,

## Evaluating the security of the system
The aim of this process is to identify and understand the possible vulnerabilities in the system and to develop the Threat Model.

The below steps were performed to achieve this goal

1. Identifying the services running on the system 

      Used **nmap** scan to find the running services and open ports. 
      
2. Identifying possible vulnerablities in the system
      
      a. **NESSUS** scan was performed to do a priliminary scan of the running services and to find vulnerable services, if any
      
      b. The flaws in the services running in the web server were identified

3. Gain access into the system by exploiting possible vulnerabilities
    
      a. Brute Forcing and SQL Injection were used to find the passwords of some users
      
      b. Dirty cow local exploit was used to gain root access
    
4. Attack Sureface was identified

5. Threat model was created

    a. Threats to open ports were identified
    
    b. STRIDE model was created 
    
    c. DREAD model was created  

## Improving the security of the system

The goal is to harden the web server to make it usable in the production environment as the Internet Gateway for a company.

1. Threat Modelling and Attack Surface Analysis were performed

2. HTTPS was setup

3. Banners were removed to eleminate any identifying information

4. Web server was jailed using Jailkit

5. Other hardening processes such as updating services, changing default passwords, etc were performed
