# Introduction

-Salesforce is a leading CRM (Customer Relationship Management) software which is served form cloud. It has more than 800 applications to support various features like generating new leads, acquiring new leads, increasing sales and closing the deals. It is designed to manage the organization's data focused on customer and sales details. It also offers features to customize its inbuilt data structures and GUI to suit the specific needs of a business. More recently, it has started offering the IOT (internet of things) connectivity to the CRM platform.

-Salesforce delivers a highly customized experience to the customers, employees, and partners of an organization. Such a platform is used to customize standard functionality and create custom pages, components, apps, etc. Also it is done faster, mainly because of the superb architecture on which it is built. Below is a brief introduction to the Salesforce Architecture.

# Benifits Of salesforce

-Reliable.

-Many tiers of security.

-24/7 Availability.

-Automation of everyday tasks.

-Provides CRM for enhanced communication

-Improves efficiency and proficiency.

# PROBLEMS WITH EXISTING SYSTEM
1 The HR usually make a list of shortlisted candidates manually with either excel spreadsheets or word. 

2 Moreover , Present system do not automate the processes.

3 Hr’s have to contact to employment websites through telephonic calls or  e-mails.

4 Hr’s find it complex to make a list of potential candidates.

# Objectives of the project
1. HR Recruiting App intends to reduce the hectic job of recruiting the employees manually.
2. Company can instantaneously upload vacancies using this app notifying the potential employees.
3. The Recruiting app make sure that a new job opening has executive approval before it becomes active. 
4. Include reports that give users an overview of recruiting status.
5. Allow recruiters to map the locations of all candidates who are applying for a position, to better understand relocation expenses.
6. Make it easy to perform several similar tasks at once, like rejecting multiple job applications.
7. Automatically post open positions on Universal Containers' public website.

# Hardware Requirements

![image](https://user-images.githubusercontent.com/53430901/117373956-df2fd900-aee9-11eb-929f-3cb2a7bb89b7.png)

# Software Requirements

![image](https://user-images.githubusercontent.com/53430901/117373979-ed7df500-aee9-11eb-9b8b-05a33ab6243d.png)

# Architectural Design

There are 2 types of objects in Salesforce: Custom Objects and Standard Objects.
Custom Objects are those objects which are made by the user itself where a while Standard objects are those which are provided by default by the Salesforce

# Modules In The App


![image](https://user-images.githubusercontent.com/53430901/117374082-20c08400-aeea-11eb-8270-ec1eca1c7580.png)

![image](https://user-images.githubusercontent.com/53430901/117374056-13a39500-aeea-11eb-9240-daea33d75ae9.png)

# Relation Design

1. There are 2 types of Relationship in Salesforce: Master-Detail and Look-up Relationship.
2. In Master-Detail Relationship , we have one parent object and multiple child objects.
3. In Lookup Relationship, this is one more category of one-to-many relationship but two objects will not put any effect on deletion or security.

![image](https://user-images.githubusercontent.com/53430901/117374266-75fc9580-aeea-11eb-827b-21d0be7171e1.png)

# Functional Design

1. The functional design phase provides a translation between the requirements analysis and the detail design. 
2. In a software development project, the functional design focuses on the general definition of the whole system or application.
3. Commonly, the functional design is confused with a technical design.

# Functional design shown in the form of Data Flow Diagrams

![image](https://user-images.githubusercontent.com/53430901/117374331-9e848f80-aeea-11eb-8c38-57e19f104746.png)

# Implementation

Implementation includes

Screenshots of project
Working of project
Various Modules in project

# Home Page

![image](https://user-images.githubusercontent.com/53430901/117374453-c96ee380-aeea-11eb-9067-3c82afbbe027.png)

# Adding a new position

![image](https://user-images.githubusercontent.com/53430901/117374478-d8559600-aeea-11eb-8fa2-301c98918dfb.png)

# Available Candidates

![image](https://user-images.githubusercontent.com/53430901/117374501-e7d4df00-aeea-11eb-916a-112ff014645c.png)

# Job Applications
![image](https://user-images.githubusercontent.com/53430901/117374533-f622fb00-aeea-11eb-9853-275780773d52.png)

# Employment Websites

![image](https://user-images.githubusercontent.com/53430901/117374568-04711700-aeeb-11eb-8d56-bc533bc34a6a.png)

# Accounts

![image](https://user-images.githubusercontent.com/53430901/117374588-0fc44280-aeeb-11eb-8fe4-5b48f9070e7a.png)

# Chatter

![image](https://user-images.githubusercontent.com/53430901/117374601-19e64100-aeeb-11eb-8b0e-a61c5fdcc986.png)

# Reports

![image](https://user-images.githubusercontent.com/53430901/117374621-223e7c00-aeeb-11eb-91dc-2ca6adb2c0cc.png)

# Dashboard

![image](https://user-images.githubusercontent.com/53430901/117374660-2c607a80-aeeb-11eb-8c4b-02585149a256.png)

# Setup Instructions

1. Login to your Salesforce Org using a System Administrator account or create a new Salesforce org.

2. If not already enabled, enable the Lightning Experience using the link found in the Setup section.

3. Install the <a href="https://login.salesforce.com/packaging/installPackage.apexp?p0=04t61000000gPxj" target="_blank">HR Demo package</a> in your Salesforce org.
   (Install for All Users)

4. Download the following CSV files and import, in the prescribed order, into your Salesforce org. using [DataLoader.io](https://dataloader.io/).
   - First import the [Job Requisition Data](https://platform-harbor-cruise.herokuapp.com/files/job-requisition-data.csv) into the **Job Requisition** object.
   - Then import the [Applicant Data](https://platform-harbor-cruise.herokuapp.com/files/applicant-data.csv) into the **Applicant** object.
   - Then import the [CIO Dashboard Data](https://platform-harbor-cruise.herokuapp.com/files/cio-dashboard-data.csv) into the **CIO Dashboard Data** object.

5. Go to **Administer > Manage Users > Profiles**, click the **System Administrator** link (typically on the second page), scroll down and click **New** in the Login IP Ranges section: Enter **0.0.0.0** for the Start IP Address and **255.255.255.255** for the End IP Address. Click **Save**.

6. Click this [![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/gabesumner/salesforce-hr-demo) button to clone this Heroku project. If you do not already have a Heroku account then sign up for a new free Heroku account, otherwise click **Log In** to use your existing account.

7. Give your new app a name (*this name will become part of the URL, example http://my-app-name.herokuapp.com*). Then use the **SALESFORCE_USERNAME** and **SALESFORCE_PASSWORD** Config Variables to enter the login credentials for your Salesforce Org (the same credentials used in Step 1).

8. *Optionally*, set the **COMPANY_NAME** and **COMPANY_LOGO** *(ideally the company logo should have a transparent background and be 40 pixels in height)*.

9. Click the **Deploy for Free** button, wait for the deployment process to finish, then click **Manage App**.

10. Click **Heroku Connect** then click **Setup Connection** to connect Heroku to your Salesforce Org. Click **Next** then select **Production** and click **Authorize**. Login to your Salesforce Org and authorize Heroku Connect to access your org's data.

11. Check the **Streaming API** checkbox and click the **Save** button.

12. Click the **Create Mapping** then select (or search for) **HR_Job_Requisition__c**. Select the following fields:
   - CreatedDate
   - HR_Description__c
   - HR_Location__c
   - HR_Status__c
   - Name

13. You're finished and can now access your website using the URL: http://your-app-name.herokuapp.com/ *(Replace "your-app-name" with your app name. If you don't know your app name then go to http://heroku.com/ and look at your Dashboard.)*

# merits

1. Morale  and motivation of employees improves.

2. Promotes loyalty and commitment  amongst employees  due to sense of job security and advancements.

3. Chances of proper selection high.

4. Present employees familiar with organization surroundings. 

5. Time and expenditure for recruitment reduced.

# Conclusion

In a bid to underscore this subtle point, the project examines the various processes and nuances of  the most critical activities of an organization. 


