This repository is the home directory of IBM Operational Decision Manager for Developers.

# IBM Operational Decision Manager for Developers - Rule Designer

## Features
Rule Designer is the Eclipse-based development environment for ODM developers. Rule Designer is needed to begin the development of a decision service. You must define a XOM and set up a vocabulary so that you can author and orchestrate business rules.

In the designer, developers can edit and debug Java code and rules alongside each other. The key features include auto correction of rules, decision flow control, code-generation wizards, source code control integration, and conflict and redundancy detection. Used with Decision Center and Rule Execution Server, Rule Designer completes a collaborative work environment for developers, business users, integrators, and release managers to automate a company's business policies.

## Installation Options

### Ready-to-Use Installation (Recommended)

We provide **three ready-to-use installation options** that come pre-configured with Eclipse and all necessary dependencies. This is the **preferred and easiest way** to get started with Rule Designer:

1. **Download the ready-to-use package** for your platform (Linux, macOS, or Windows) from the [releases page](https://github.com/DecisionsDev/ruledesigner/releases) 
2. **Extract and run** 
   - **macOS only**: Before running the RuleDesigner.app , remove the quarantine attribute by running the following command:
       ```
        xattr -r -d com.apple.quarantine RuleDesigner.app
     ```
4. **Start developing** - Eclipse with Rule Designer is ready to use immediately
   - ruledesigner.exe (Windows)
   - RuleDesigner.App (Mac OS)
   - ruledesigner (Linux) 

Available versions:
- **[9.6](https://github.com/DecisionsDev/ruledesigner/releases/tag/v9.6.0)** - Eclipse 2025-12 (4.38) with JDK 21


### Alternative Installation Methods

If you prefer to install Rule Designer into an existing Eclipse installation, refer to the official documentation:

- **[Installing Rule Designer online](https://www.ibm.com/docs/en/SSQP76_9.6.0/com.ibm.odm.kube/topics/tsk_install_designer.html)** - Install Rule Designer in Eclipse from the Eclipse Marketplace
- **[Installing Rule Designer offline](https://www.ibm.com/docs/en/SSQP76_9.6.0/com.ibm.odm.kube/topics/tsk_install_designer_ol.html)** - Download Rule Designer from GitHub and install it into Eclipse

**Available update site URLs for online installation:**
- **9.6**: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/9.6.0/p2
- **9.5**: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/9.5.0/p2
- **9.0**: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/9.0.0/p2
- **8.12.0.1**: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/8.12.0/p2
- **8.11.1**: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/8.11.1/p2
- **8.11.0.1**: https://raw.githubusercontent.com/DecisionsDev/ruledesigner/8.11.0.1/p2

## Configuration

### Display Modes
Rule Designer supports different display modes to match your preferences. Learn more about [display modes](https://www.ibm.com/docs/en/SSQP76_9.6.0/com.ibm.odm.kube/shared_config_topics/con_theme_mode.html) (classic, dark, and light).

### Security Certificate Import
To securely connect Rule Designer to Decision Server and Decision Center services running in Certified Kubernetes, you need to establish a TLS connection through a security certificate. 

See the detailed guide: 
- For **ODM on certified Kubernetes**: [Importing a security certificate in Rule Designer](https://www.ibm.com/docs/en/odm/9.6.0?topic=designer-importing-security-certificate-in-rule)
- For **Cloud Pak for Business Automation**: [CP4BA - Importing a security certificate in Rule Designer](https://www.ibm.com/docs/en/cloud-paks/cp-biz-automation/26.0.0?topic=manager-importing-security-certificate-in-rule-designer)

> **Note:** On some macOS installations, you may encounter issues when importing a security certificate in Rule Designer. For detailed troubleshooting steps and tips, refer to the [IBM Community article on importing a security certificate](https://community.ibm.com/community/user/automation/blogs/sia-sin-tay/2025/01/13/tips-about-importing-a-security-certificate-in-rul) in Rule Designer.


# Issues and Contributions
For issues relating specifically to this project and scripts, please use the [GitHub issue tracker](https://github.com/DecisionsDev/ruledesigner/issues).

# License
The files found in this project are licensed under the [IBM Operational Decision Manager for Developers license](LICENSE).

# Copyright
© Copyright IBM Corporation 2026.
