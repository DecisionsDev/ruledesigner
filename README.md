This repository is the home directory of IBM Operational Decision Manager for Developers.

# IBM Operational Decision Manager for Developers - Rule Designer

## Features
Rule Designer is the Eclipse-based development environment for ODM developers. Rule Designer is needed to begin the development of a decision service. You must define a XOM and set up a vocabulary so that you can author and orchestrate business rules.

In the designer, developers can edit and debug Java code and rules alongside each other. The key features include auto correction of rules, decision flow control, code-generation wizards, source code control integration, and conflict and redundancy detection. Used with Decision Center and Rule Execution Server, Rule Designer completes a collaborative work environment for developers, business users, integrators, and release managers to automate a company's business policies.

## Requirements
For 8.9.2 Release:
 - Eclipse 4.4 Luna Packages
 - You can find all available releases at this location : https://github.com/ODMDev/ruledesigner/releases

For 8.10.0 Release:
 - Eclipse 4.7 Oxygen Packages
 - You can find all available releases at this location : https://github.com/ODMDev/ruledesigner/releases

For 8.10.1 Release:
 - Eclipse 4.7.3 Oxygen Packages
 - You can find all available releases at this location : https://github.com/ODMDev/ruledesigner/releases

 For 8.10.2 Release:
  - Eclipse 4.7.3 Oxygen Packages
  - You can find all available releases at this location : https://github.com/ODMDev/ruledesigner/releases


## Installation
You must install the update site for Rule Designer into an existing Eclipse.

1. Start Eclipse.
2. Switch to the **Java** perspective (click **Window** > **Open Perspective** > **Java**).
3. Click **Help** > **Install New Software**.
4. Add the update site to install:
   - In the Install wizard, next to the **Work with** field, click **Add**.
   - In the **Name** field, enter a name for the repository. For example, enter Rule Designer.
   - In the **Location** field, enter
   		- For 8.9.2:  https://raw.githubusercontent.com/ODMDev/ruledesigner/8.9.2/p2 .
   		- For 8.10.0:  https://raw.githubusercontent.com/ODMDev/ruledesigner/8.10.0/p2 .
      - For 8.10.1: https://raw.githubusercontent.com/ODMDev/ruledesigner/8.10.1/p2 .
      - For 8.10.2: https://raw.githubusercontent.com/ODMDev/ruledesigner/8.10.2/p2 .

   - Click **OK**.
5. Click **Select All**, and click **Next**. Eclipse calculates the dependencies and requirements.
6. In the **Install** dialog, click **Next**.
7. In the **Review Licenses** dialog, select `I accept the terms of the license agreement`, and then click **Finish**. The installation might take a few seconds to complete. If a security warning about the validity of the software opens, click **OK** to proceed with the installation.
8. If you are prompted to restart Eclipse, click **Yes**.
9. If not displayed by default, switch to the **Rule** perspective (**Window** > **Open Perspective** > **Rule**).

## What to do next
If you want to establish a secure TLS connection with ODM for dev on IBM Cloud Private, you need to import a certificate into the cacerts file in the JVM used to launch Rule Designer.

ODM on IBM Cloud Private is delivered with a [default certificate](odmonicpserver.cer). To connect to ODM on ICP with this certificate, you must copy the file to the JVM used to launch Rule Designer.

To add the `odmonicpserver.cer` certificate to the JVM's default cacerts truststore, use the keystore keytool:
```
cd <JAVA_HOME>/jre/lib/security
keytool -importcert -file odmonicpserver.cer -keystore cacerts -storepass changeit -alias odmicpserver
```
**Where** `changeit` is the password to protect the integrity of the `cacerts` file.

You can also use the [truststore.jks](truststore.jks) file, which contains the `odmonicpserver.cer` certificate. To use the truststore in Rule Designer, copy the `truststore.jks` file to your Rule Designer installation directory next to the `eclipse.ini` file, add the following lines at the end of your `eclipse.ini` file, and then restart Rule Designer.
```
-Djavax.net.ssl.trustStore=truststore.jks
-Djavax.net.ssl.trustStorePassword=changeme
```
**Where** `changeme` corresponds to the password for the default `truststore.jks` file.

# Issues and contributions
For issues relating specifically to this project and scripts, please use the [GitHub issue tracker](../../issues).

# License
The files found in this project are licensed under the [IBM Operational Decision Manager for Developers license](LICENSE).

# Copyright
© Copyright IBM Corporation 2019.
