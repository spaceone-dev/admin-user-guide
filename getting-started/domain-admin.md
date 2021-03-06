---
description: >-
  The role of Domain Admin creates the top-level project group, creates users,
  and sets the main collector.
---

# Domain Admin

## Sign-in

**STEP 1:** Drive to domain of **SpaceONE** on browser ****and type given ID and Password as domain admin.  
**\(**E-mail received from the Root Account has stated detailed the connection methods; Single Sign On\(SSO\),  ID/PW, or Google Oauth2**\)**

![](../.gitbook/assets/screen-shot-2021-02-04-at-14.39.08.png)

## Create Project Group

All cloud resources **MUST** belong to a certain project for management purposese. You can grouping any projects with Project Group.   
Domain Admin creates the project group based on the company's management policy.

{% hint style="info" %}
**Note&gt;** General User **\(Project Admin\)** creates projects only under project group with permission to manage cloud resources.   
{% endhint %}

**STEP 1:** Drive to menu **`Project`** at the top menu bar and click **`+ Create Group button`** of the panel.

![](../.gitbook/assets/create_top_project_group.png)

**STEP 2:** Type project group name \(**sample case: Landing Zone**\) and Click Confirm.

![](../.gitbook/assets/create_project_group_landingzone.png)

**STEP 3:** Type project group name \(**sample case: Services**\) and click Confirm.

![](../.gitbook/assets/create_project_group_services.png)

**STEP 4:** Type project group name \(**sample case: Business Support Systems**\) and click Confirm.

![](../.gitbook/assets/create_project_group_businesssupportsystems.png)

**STEP 5:** Check all 3 project groups have created a tree on the left menu.

![](../.gitbook/assets/show_project_page.png)

## Create User

Create general users and assign the project groups to the created user. General users can access only the project group to which they are belonged to.

**STEP 1:** Drive to menu **`Identity > User`** at the top bar. 

![](../.gitbook/assets/screen-shot-2021-02-04-at-14.16.22%20%281%29.png)

  
**STEP 2:** Click **`+ Add`** button to add a domain Admin user.

![](../.gitbook/assets/screen-shot-2021-02-04-at-14.18.45%20%281%29.png)

**STEP 3:** Fill out all required fields ****and click **`Confirm`** button once finish.

![](../.gitbook/assets/create_user1-1-.png)

**STEP 4:** Drive to Project ****and click **MEMBER** icons at right next to **`+ Create Project`** button.

![](../.gitbook/assets/screen-shot-2021-02-04-at-16.28.10.png)

**STEP 5:** Click **`+ Add`** button and select members to add to the project group on the list at the pop-up window.

![](../.gitbook/assets/screen-shot-2021-02-05-at-10.11.22.png)

**STEP 6:** Click **`Confirm`** button when you finish to all members and set their role as project admin.

![](../.gitbook/assets/add_user2_to_project_group.png)

\*\*\*\*

**STEP 7:** Check all selected members have registered as project members.

![](../.gitbook/assets/screen-shot-2021-02-05-at-10.17.46.png)

## Cloud Resource Collectors

**Cloud Resource Collector** \(a.k.a **CRC**\) is a plugin that collects cloud resources across platforms such as AWS, Google Cloud, Azure, CRC is set by Domain Admin only.

**STEP 1:** Drive to Menu **`Plugin > Collector`**and Click **`+ Create`**button.

![](../.gitbook/assets/create_collector.png)



### **Create AWS EC2 Collector**

**STEP 1:** Select **AWS-ec2** plugin and Click **`+ Create`** Button. ****

\*\*\*\*

![](../.gitbook/assets/select_aws_ec2_plugin.png)

**STEP 2:** Please, fill out all required fields and select drop downs for each steps \(**add tags** is optional\) and Click **`Confirm`** button to create **AWS EC2 collector**.

![](../.gitbook/assets/create_aws_personal_health_dashboard_collector.png)



### **Create AWS Cloud Services Collector** 

**STEP 1:** Select AWS**-cloud-services** plugin and Click **`+ Create`** Button. ****

![](../.gitbook/assets/select_aws_cloud_services_plugin-1-%20%282%29.png)

  
**STEP 2:** Please, fill out all required fields and select drop downs for each steps \(**Add Tags** is Optional\) and Click **`Confirm`** button to create **AWS Cloud Service Collecto**r.

![](../.gitbook/assets/screen-shot-2021-02-05-at-13.46.13.png)

\*\*\*\*

### **Create AWS  Trusted Advisor Collector** 

**STEP 1:** Select **AWS-trusted-advisor** plugin and Click **`+ Create`** Button. ****

![](../.gitbook/assets/screen-shot-2021-02-05-at-13.53.03%20%281%29.png)

**STEP 2:** Please, fill out all required fields and select drop downs for each steps \(**add Tags** is optional\) and Click **`Confirm`** button to create **AWS Trusted Advisor collecto**r.

![](../.gitbook/assets/create_aws_trusted_advisor_collector.png)

\*\*\*\*

### **Create AWS Health Dashboard Collector** 

**STEP 1:** Select **AWS-personal-health-dashboard** plugin and Click **`+ Create`** Button. ****

![](../.gitbook/assets/select_aws_cloud_services_plugin-1-%20%281%29.png)

**STEP 2:** Please, fill out all required fields and select drop downs for each steps \(**add Tags** is optional\) and Click **`Confirm`** button to create **AWS Health Dashboard collector**.

![](../.gitbook/assets/create_aws_personal_health_dashboard_collector%20%281%29.png)

\*\*\*\*

### **Create Monitoring Metric Collector** 

**STEP 1:** Select **monitoring-metric-collector** plugin and Click **`+ Create`** Button. ****

![](../.gitbook/assets/select_aws_cloud_services_plugin-1-.png)

**STEP 2:** Please, fill out all required fields and select drop downs for each steps \(**add Tags** is optional\) and click **`Confirm`** button.

![](../.gitbook/assets/screen-shot-2021-02-05-at-13.46.13%20%281%29.png)

**FINAL STEP:** Check all created collectors on the collector list.

![](../.gitbook/assets/screen-shot-2021-02-05-at-13.53.03.png)

## Set collection schedule

The schedule is to set the collection time so that the collectors run the jobs periodically to collect cloud resources.

**STEP 1:** Click the **Schedule** tab on the bottom\(detail\) page of the selected collector.

![](../.gitbook/assets/screen-shot-2021-02-05-at-14.02.50.png)

**STEP 2:**  Click **`+ Add`** button; Fill out Name and Time zone, and Select Schedule Frequency and then Click **`Confirm`** button once the schedule setting is finished. 

{% hint style="info" %}
1. Set '**Hourly schedule**' which runs everyday at selected hour 
2. Set '**Repeat Every \***' which runs every given intervals in seconds, minutes or hours.
{% endhint %}

![](../.gitbook/assets/add_schedule_to_collector.png)



  
**STEP3:** Check whether the collector schedule is registered on the collector.

![](../.gitbook/assets/list_collector_schedules.png)

