# Patch Manager Prerequisites<a name="patch-manager-prerequisites"></a>

**SSM Agent Version**  
Version 2\.0\.834\.0 or later of SSM Agent be running on the instances you want to manage with Patch Manager\.

**Note**  
SSM Agent is updated whenever changes are made to Systems Manager and when new capabilities are added\. To ensure that your instances are always running the newest version of SSM Agent, we recommend that you create a State Manager association that automatically updates SSM Agent when a new version is available\. You can also use Run Command to quickly update one or more instances with the latest version\. For more information, see [Automatically Update SSM Agent \(CLI\)](sysman-state-cli.md) \(State Manager\) and [Update SSM Agent by using Run Command](rc-console.md#rc-console-agentexample)\.

**Supported Operating Systems**  
The Patch Manager capability does not support all the same operating systems versions that are supported by other AWS Systems Manager capabilities\. For example, Patch Manager does not support CentOS 6\.3, Raspbian Stretch, or Windows Server 2003\. \(For the full list of Systems Manager\-supported operating systems, see [Systems Manager Prerequisites](systems-manager-prereqs.md)\.\) Therefore, ensure that the instances you want to use with Patch Manager are running one of the operating systems listed in the following table\.


| Operating System | Details | 
| --- | --- | 
|  Linux  | [\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/systems-manager/latest/userguide/patch-manager-prerequisites.html)  Instances created from an Amazon Linux AMI that are using a proxy must be running a current version of the Python `requests` module in order to support Patch Manager operations\. For more information, see [Upgrade the Python Requests Module on Amazon Linux Instances That Use a Proxy Server](sysman-proxy-with-ssm-agent-al-python-requests.md)\.  | 
|  Windows  |  Windows Server 2008 through Windows Server 2019, including R2 versions\.  | 