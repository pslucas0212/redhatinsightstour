# The Insights Tour for Red Hat Enterprise Linux
Updated 1 June 2021

A tour of using Red Hat Insights with Red Hat Enterprise Linux

### Introduction
In this tutorial, we will be focusing on the Red Hat Enterprise Linux portion of Red Hat Insights.  Red Hat Insights (RHI) is part of your Red Hat Enterprise Linux (RHEL) subscription and supports RHEL 6.4+, 7.0+, and 8.0+.  

From the Red Hat Insights FAQ (see link below): "Red Hat Insights is a Red Hat software-as-a-service(SaaS) offering that helps IT teams proactively identify and remediate threats to security, performance, availability, and stability. Before subscribers need to come to Red Hat’s customer portal to troubleshoot, investigate, or learn how to avoid issues, outages, and unplanned downtime, Insights uses software to ensure their entire Red Hat Enterprise Linux environment is operating optimally. No other Linux provider offers this type of proactive, automated, and targeted resolution to ensure a secure, reliable, efficient, and scalable infrastructure environment."

### Setting Up RHEL with Insights
Register RHEL to the RHSM Service
- You will need to have your RHEL instance Registered with the Red Hat Subscription Manager to access RHI.  See the following examples to register a system via subscription manager for RHEL 6.0+, 7.0+ and 8.0+.  Note: You will need to use sudo or be root to execute these commands.

      # subscription-manager register --org=xxxxxxxxx --activationkey=your_key_here
      
- Verify that the registered system content access mode is set to SCA.  Note: You will only see the SCA status on RHEL 7.0+ and 8.0+

      # subscription-manager status
      
Enable the RHI client.
- Insights setup for RHEL 8

      # insights-client --enable
      
- Insights setup for RHEL 6.4+ and 7.0+

      # yum -y install insights-client
      # insights-client --enable
        

### References

- [Registration Assistant](https://access.redhat.com/labs/registrationassistant/)
- [Red Hat Insights FAQ](https://access.redhat.com/articles/4602981)
- [Insights-client Configuration Options for Red Hat Insights ](https://access.redhat.com/articles/4099591)
- 

Note: Red Hat continues to add new features and enhance the Red Hat Insights user experience.  Some of the screen shot and UI navigation instructions from older articles may not map directly to the current Red Hat Insights UI.

- [Simplify troubleshooting RHEL system configurations with Red Hat Insights Drift service ](https://www.redhat.com/en/blog/simplify-troubleshooting-rhel-system-configurations-red-hat-insights-drift-service?channel=blog/channel/red-hat-insights)
- [Defense in depth with Red Hat Insights](https://www.redhat.com/en/blog/defense-depth-red-hat-insights?channel=blog/channel/red-hat-insights) - February 24, 2021
- [Integrating a monitoring system with Red Hat Insights](https://www.redhat.com/en/blog/integrating-monitoring-system-red-hat-insights?channel=blog/channel/red-hat-insights) - January 11, 2021
- [Red Hat Insights feature highlights: Exploring historical system profiles in Drift for easier RHEL configuration troubleshooting](https://www.redhat.com/en/blog/red-hat-insights-feature-highlights-exploring-historical-system-profiles-drift-easier-rhel-configuration-troubleshooting?channel=blog/channel/red-hat-insights) - October 19, 2020
- [Getting started with the Red Hat Insights policies capability](https://www.redhat.com/en/blog/getting-started-red-hat-insights-policies-capability?channel=blog/channel/red-hat-insights&page=1) - September 23, 2020
- [Managing the security of your Red Hat Enterprise Linux environment with Red Hat Insights](https://www.redhat.com/en/blog/managing-security-your-red-hat-enterprise-linux-environment-red-hat-insights?channel=blog/channel/red-hat-insights&page=1) - September 17, 2020
- [Getting started with the Red Hat Insights patch capability](https://www.redhat.com/en/blog/getting-started-red-hat-insights-patch-capability?channel=blog/channel/red-hat-insights&page=1) - September 9, 2020
- [Introducing Red Hat Insights Drift Capability for Red Hat Enterprise Linux configuration troubleshooting](https://www.redhat.com/en/blog/introducing-red-hat-insights-drift-capability-red-hat-enterprise-linux-configuration-troubleshooting?channel=blog/channel/red-hat-insights&page=1) - August 24, 2020
- [Red Hat Insights delivers easier RHEL management with Red Hat knowledge base integration and enhanced customer portal applications](https://www.redhat.com/en/blog/red-hat-insights-delivers-easier-rhel-management-red-hat-knowledge-base-integration-and-enhanced-customer-portal-applications?channel=blog/channel/red-hat-insights&page=1) - August 11, 2020
- [Redefining RHEL: Introduction to Red Hat Insights - 2020 Update](https://www.redhat.com/en/blog/redefining-rhel-introduction-red-hat-insights?channel=blog/channel/red-hat-insights&page=1) - July 30, 2020
- [New Role Based Access Control for Red Hat Insights for Red Hat Enterprise Linux](https://www.redhat.com/en/blog/new-role-based-access-control-red-hat-insights-and-cloud-management-services-red-hat-enterprise-linux?channel=blog/channel/red-hat-insights&page=2) - March 17, 2020
- [Modernizing Red Hat Enterprise Linux System management the easy way](https://www.redhat.com/en/blog/modernizing-red-hat-enterprise-linux-system-management-easy-way?channel=blog/channel/red-hat-insights&page=2) - January 14, 2020
- [What’s new in Red Hat Insights for November, 2019?](https://www.redhat.com/en/blog/whats-new-red-hat-insights-november-2019?channel=blog/channel/red-hat-insights&page=2) - November 5, 2019

