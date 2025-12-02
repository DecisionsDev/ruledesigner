This repository is the home directory of IBM Operational Decision Manager for Developers.

# IBM Operational Decision Manager for Developers - Rule Designer

## Features
Rule Designer is the Eclipse-based development environment for ODM developers. Rule Designer is needed to begin the development of a decision service. You must define a XOM and set up a vocabulary so that you can author and orchestrate business rules.

In the designer, developers can edit and debug Java code and rules alongside each other. The key features include auto correction of rules, decision flow control, code-generation wizards, source code control integration, and conflict and redundancy detection. Used with Decision Center and Rule Execution Server, Rule Designer completes a collaborative work environment for developers, business users, integrators, and release managers to automate a company's business policies.

## Requirements

For 8.11.0.1 Release:
   - Eclipse IDE 2020-06 R (4.16) Modeling Tools Packages
   - JDK 8

For 8.11.1 Release:
   - Eclipse IDE 2020-06 R (4.16) Modeling Tools Packages
   - JDK 8

For 8.12.0.1 Release:
   - Eclipse IDE 2022-06 R (4.24) Modeling Tools Packages
   - JDK 11

For 9.0 Release:
   - Eclipse IDE 2023-12 R (4.30) Eclipse IDE for Enterprise Java and Web Developers Packages
   - JDK 17

For 9.5 Release:
   - Eclipse IDE 2024-12 R (4.34) Eclipse IDE for Enterprise Java and Web Developers Packages
   - JDK 21
> 
> **Mandatory** before installing Rule Designer 
>
> 1. Start Eclipse
> 2. Open Window > Preferences > Install > Update > Available software sites.
>    Disable all the sites except the following:
>    - https://download.eclipse.org/releases/2024-12
>    - https://download.eclipse.org/eclipse/updates/4.34
> 3. Click Apply > Close.
  
     
## Installation
You must install the update site for Rule Designer into an existing Eclipse.
1. Start Eclipse.
2. Switch to the **Java** perspective (click **Window** > **Open Perspective** > **Java**).
4. Click **Help** > **Install New Software**.
5. Add the update site to install:
   - In the Install wizard, next to the **Work with** field, click **Add**.
   - In the **Name** field, enter a name for the repository. For example, enter Rule Designer.
   - In the **Location** field, enter
     - For 8.11.0.1: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/8.11.0.1/p2 .
     - For 8.11.1: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/8.11.1/p2 .
     - For 8.12.0.1: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/8.12.0/p2 .
     - For 9.0 : https://raw.githubusercontent.com/DecisionsDev/ruledesigner/9.0.0/p2 .
     - For 9.5 : https://raw.githubusercontent.com/DecisionsDev/ruledesigner/9.5.0/p2 .     
   - Click **OK**.
6. Click **Select All**, and click **Next**. Eclipse calculates the dependencies and requirements.
7. In the **Install** dialog, click **Next**.
8. In the **Review Licenses** dialog, select `I accept the terms of the license agreement`, and then click **Finish**. If a security warning about the validity of the software opens, click **OK** to proceed with the installation.
9. During the installation, you will be prompted with a **Trusted Authorities** dialog, select `https://raw.githubusercontent.com` in **Authoring / Update site** section and then click **Trust Selected** to continue.
10. A **Trust Artifacts** dialog will be prompted a few moment later, click **Select All** and then click **Trust Selected** to continue the installation. The installation might take a few seconds to complete. 
11. If you are prompted to restart Eclipse, click **Yes**.
12. If not displayed by default, switch to the **Rule** perspective (**Window** > **Open Perspective** > **Rule**).

## Offline installation
1. Go to the https://github.com/DecisionsDev/ruledesigner/releases
2. Download source code
3. Uncompress it on your local machine
4. Start Eclipse
5. Switch to the **Java** perspective (click **Window** > **Open Perspective** > **Java**).
6. Click **Help** > **Install New Software**.
7. Add the update site to install:
   - In the Install wizard, next to the **Work with** field, click **Add**.
   - In the **Name** field, enter a name for the repository. For example, enter Rule Designer.
   - Click Local select the p2 folder in the uncompress directory.
8. Click **Select All**, and click **Next**. Eclipse calculates the dependencies and requirements.
9. In the **Install** dialog, click **Next**.
10. In the **Review Licenses** dialog, select `I accept the terms of the license agreement`, and then click **Finish**. If a security warning about the validity of the software opens, click **OK** to proceed with the installation.
11. During the installation, you will be prompted with a **Trusted Authorities** dialog, select `https://raw.githubusercontent.com` in **Authoring / Update site** section and then click **Trust Selected** to continue.
12. A **Trust Artifacts** dialog will be prompted a few moment later, click **Select All** and then click **Trust Selected** to continue the installation. The installation might take a few seconds to complete. 
13. If you are prompted to restart Eclipse, click **Yes**.
14. If not displayed by default, switch to the **Rule** perspective (**Window** > **Open Perspective** > **Rule**).

## What to do next
If you want to establish a secure TLS connection or/and use an OpenID provider with ODM on Kubernetes, you need to import a certificate into the cacerts file and configure the OpenID provider in the JVM used to launch Rule Designer. 
Steps to configure Rule Designer are explains :
- In the [Cloud Pak for Business Automation 25.0.0 ](https://www.ibm.com/docs/en/cloud-paks/cp-biz-automation/25.0.0?topic=manager-importing-security-certificate-in-rule-designer) documentation
- In the [Operational Decision Manager for Kubernetes 9.5.0](https://www.ibm.com/docs/en/odm/9.5.0?topic=designer-importing-security-certificate-in-rule) documentation

> Note: On some macOS installations, you may encounter issues when importing a security certificate in Rule Designer. For detailed troubleshooting steps and tips, refer to the [IBM Community article on importing a security certificate](https://community.ibm.com/community/user/automation/blogs/sia-sin-tay/2025/01/13/tips-about-importing-a-security-certificate-in-rul) in Rule Designer. This guide provides specific instructions that can help resolve macOS-specific challenges.

# Issues and contributions
For issues relating specifically to this project and scripts, please use the [GitHub issue tracker](https://github.com/DecisionsDev/ruledesigner/issues).

# License
The files found in this project are licensed under the [IBM Operational Decision Manager for Developers license](LICENSE).

# Copyright
© Copyright IBM Corporation 2025.
