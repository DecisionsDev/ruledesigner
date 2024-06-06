This repository is the home directory of IBM Operational Decision Manager for Developers.

# IBM Operational Decision Manager for Developers - Rule Designer

## Features
Rule Designer is the Eclipse-based development environment for ODM developers. Rule Designer is needed to begin the development of a decision service. You must define a XOM and set up a vocabulary so that you can author and orchestrate business rules.

In the designer, developers can edit and debug Java code and rules alongside each other. The key features include auto correction of rules, decision flow control, code-generation wizards, source code control integration, and conflict and redundancy detection. Used with Decision Center and Rule Execution Server, Rule Designer completes a collaborative work environment for developers, business users, integrators, and release managers to automate a company's business policies.

## Requirements

For 9.0.0 Release:
   - Eclipse IDE 2023-12(4.30) Modeling Tools Packages uses Java Development Kit (JDK) 17.
   - You can find all available releases at this location : https://github.com/ODMDev/ruledesigner/releases
   - You can download the JDK from [IBM Semeru Runtimes Downloads](https://developer.ibm.com/languages/java/semeru-runtimes/downloads/).


## Installation
You must install the update site for Rule Designer into an existing Eclipse.

1. Start Eclipse.
2. Switch to the **Java** perspective (click **Window** > **Open Perspective** > **Java**).
3. Click **Help** > **Install New Software**.
4. Add the update site to install:
   - In the Install wizard, next to the **Work with** field, click **Add**.
   - In the **Name** field, enter a name for the repository. For example, enter Rule Designer.
   - In the **Location** field, enter
     - For 9.0.0 (And future IFix): https://raw.githubusercontent.com/ODMDev/ruledesigner/9.0.0/p2 .
     
   - Click **OK**.
5. Click **Select All**, and click **Next**. Eclipse calculates the dependencies and requirements.
6. In the **Install** dialog, click **Next**.
7. In the **Review Licenses** dialog, select `I accept the terms of the license agreement`, and then click **Finish**. The installation might take a few seconds to complete. If a security warning about the validity of the software opens, click **OK** to proceed with the installation.
8. If you are prompted to restart Eclipse, click **Yes**.
9. If not displayed by default, switch to the **Rule** perspective (**Window** > **Open Perspective** > **Rule**).

## What to do next
If you want to establish a secure TLS connection or/and use an OpenID provider with ODM on Kubernetes, you need to import a certificate into the cacerts file and configure the OpenID provider in the JVM used to launch Rule Designer. 
Steps to configure Rule Designer are explains :
- In the [Cloud Pak for Business Automation 24.0.0 ](https://www.ibm.com/docs/en/cloud-paks/cp-biz-automation/24.0.0?topic=manager-importing-security-certificate-in-rule-designer) documentation
- In the [Operational Decision Manager for Kubernetes 9.0.0](https://www.ibm.com/docs/en/odm/9.0.0?topic=designer-importing-security-certificate-in-rule) documentation


# Issues and contributions
For issues relating specifically to this project and scripts, please use the [GitHub issue tracker](../../issues).

# License
The files found in this project are licensed under the [IBM Operational Decision Manager for Developers license](LICENSE).

# Copyright
© Copyright IBM Corporation 2024.
