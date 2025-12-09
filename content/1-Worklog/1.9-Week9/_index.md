---
title: "Week 9 Worklog"
date: "2025-11-03"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Learn to use tags to organize and manage AWS resources  
* Practice creating Resource Groups and filtering resources using tags  
* Manage EC2 access using resource tags and IAM policies  
* Understand IAM permission boundaries to limit user permissions  

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 1   | - **Lab 27:** Manage Resources Using Tags and Resource Groups <br>&emsp;2. Using Tags <br>&emsp;2.1 Use tags on Console <br>&emsp;&emsp;- 2.1.1 Create EC2 instance with tag <br>&emsp;&emsp;- 2.1.2 Manage tags on AWS resources <br>&emsp;&emsp;- 2.1.3 Filter resources by tag <br>&emsp;2.2 Use tags with CLI <br>&emsp;3. Create a Resource Group <br>&emsp;4. Clean up resources | 03/11/2025 | 03/11/2025 | <https://000027.awsstudygroup.com/> |
| 2   | - **Lab 28:** Manage access to EC2 services with resource tags through IAM services <br>&emsp;1. Introduction <br>&emsp;2. Preparation <br>&emsp;&emsp;- 2.1 Create IAM user <br>&emsp;3. Create IAM Policy <br>&emsp;4. Create IAM Role <br>&emsp;5. Check Policy: <br>&emsp;&emsp;- 5.1 Switch Roles <br>&emsp;&emsp;- 5.2 Check IAM Policy <br>&emsp;&emsp;- 5.2.1 Access EC2 console in Tokyo Region <br>&emsp;&emsp;- 5.2.2 Access EC2 console in North Virginia Region <br>&emsp;&emsp;- 5.2.3 Create EC2 instance with/without required tags <br>&emsp;&emsp;- 5.2.4 Edit resource tag on EC2 instance <br>&emsp;&emsp;- 5.2.5 Policy check results <br>&emsp;6. Clean up resources | 04/11/2025 | 04/11/2025 | <https://000028.awsstudygroup.com/> |
| 3   | - **Practice:** Review Lab 27 & Lab 28 <br>&emsp;+ Repeat using tags on Console and CLI <br>&emsp;+ Practice filtering resources and using Resource Groups <br>&emsp;+ Practice tag-based access control for EC2 with IAM policies <br>&emsp;+ Note simple best practices for tags and access control | 05/11/2025 | 05/11/2025 | <https://000027.awsstudygroup.com/>, <https://000028.awsstudygroup.com/> |
| 4   | - **Lab 30:** Limitation of user rights with IAM Permission Boundary <br>&emsp;1. Introduction <br>&emsp;2. Preparation <br>&emsp;3. Create restriction policy (permission boundary) <br>&emsp;4. Create IAM limited user <br>&emsp;5. Test IAM user limits <br>&emsp;6. Clean up resources | 06/11/2025 | 06/11/2025 | <https://000030.awsstudygroup.com/> |
| 5   | - **Practice:** Review Tag, IAM Policy, and Permission Boundary <br>&emsp;+ Review how tags and Resource Groups help manage resources <br>&emsp;+ Review tag-based access control to EC2 from Lab 28 <br>&emsp;+ Review IAM permission boundary from Lab 30 <br>&emsp;+ Summarize what was learned in Week 9 | 07/11/2025 | 07/11/2025 | <https://000027.awsstudygroup.com/>, <https://000028.awsstudygroup.com/>, <https://000030.awsstudygroup.com/> |

### 🏆 **Week 9 Achievements**

* **Tags and Resource Management**
  * Used tags in the AWS Console to label EC2 and other resources
  * Filtered resources by tags for easier discovery
  * Used the AWS CLI to manage tags and create Resource Groups

* **Tag-based Access Control for EC2**
  * Created IAM user, policy, and role for tag-based access control
  * Tested EC2 console access across Regions (Tokyo, N. Virginia)
  * Tested creating EC2 instances with and without required tags
  * Edited resource tags to observe policy allow/deny behavior

* **IAM Permission Boundaries**
  * Created a restriction policy to use as a permission boundary
  * Created an IAM user with limited permissions
  * Tested the user's allowed and disallowed actions in the AWS console

* **Practice and Cleanup**
  * Practiced using tags, Resource Groups, and IAM policies multiple times
  * Cleaned up lab resources after finishing
  * Gained a clearer understanding of how tags and IAM work together to control access
