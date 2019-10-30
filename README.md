### Metadata-Backup
1.  Build a package.xml using the [Salesforce Toolkit](https://packagebuilder.herokuapp.com/) for the organization you want to back up.
How to Pull Metadata Backup From Workbench: Step-by-Step Instructions

2. Navigate to workbench.developerforce.com.

3.  Choose the environment:
Production – used for production environments as well as developer environments
Sandbox –  used for all types of sandbox environments

4.  Choose the API version that matches the version for which you generated your package.xml file:
37.0 – this is the current version of Salesforce, Summer ‘16
36.0 – Spring ‘16
35.0 – Winter ‘16
34.0 – Summer ‘15
33.0, etc. – each release of Salesforce has a different API version
 

5.  Check “I agree to the terms of service.”
 
6.  Click “Login with Salesforce”

7.  Enter the username and password for the environment
Note: If you’re currently logged into Salesforce in the same browser in which you have Workbench open, you can skip to the next step. Log out of other orgs if you do not want to use Workbench with them, or open Workbench in another browser.

8.  Navigate to the “Retrieve” UI

9.  In the “Jump To” picklist, choose “Retrieve” and click “Select”

10.  In the Migration menu in the nav bar, click “Retrieve”

11.  For “Unpackaged Manifest,” choose your package.xml file (as discussed above)

Leave “Package Names” empty
Leave “Single Package” false

12.  Click “Next”

13.  Once you have successfully staged the request, click “Retrieve”

Review and download results
Note: The page will continue to refresh until the request passes or fails.
Results at the bottom of the page give you information on your retrieve request:
Done – this will be true when the results are ready

ID – this is the ID of the operation that was performed

Status – this will be “succeeded” or “failed,” based on the operation results

Success – this will be true if the retrieve is done, succeeded, and the manifest file successfully pulled down the metadata into a zip file

FileProperties – these are all of the metadata components that were pulled with the retrieve; you can preview them before you download the file

Messages – these messages give you insight into the retrieve operations results; e.g., some metadata types may not exist in the API version chosen, may not have any components to retrieve, or may not be available in the environment that you are pulling

14.  When the retrieve passes, a zip file will be ready for download; click “Download Zip File” to get your backup
 


 
