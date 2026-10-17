# AWS-BUDGET-CONFIGURATION
Configuration files and scripts for managing and monitoring AWS budgets and cost controls

Begin by granting the target user account access from your root account

Without updated permissions, attempting to access this information will trigger errors, as seen in the screenshot below:  

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/850c2942-dd64-4247-98ab-c29fb4bf3b1f" />

From your root account, you want to click the drop-down arrow on your username and select Account

<img width="958" height="1073" alt="image" src="https://github.com/user-attachments/assets/7390e9fd-e285-48a9-a236-bb193e5a41d8" />

Once the page has loaded, scroll down until you see: IAM user and role access to Billing information, and right-click Edit

<img width="960" height="1080" alt="image" src="https://github.com/user-attachments/assets/df43c0fc-e24c-4308-9ea7-c7238c63e14f" />

This setting is currently deactivated and needs to be activated to give the user and role access to the Billing information. Check the box that states: Activate IAM Access, and click on the Update button

<img width="528" height="278" alt="image" src="https://github.com/user-attachments/assets/01025f07-f62d-4e82-aeb3-4530a607baa0" />

Your settings should now be successfully updated

<img width="527" height="307" alt="image" src="https://github.com/user-attachments/assets/0c92cfca-ed86-4497-b99c-831fccf1c236" />

You can now switch back to the user and account and refresh the page. After some time, the error messages previously seen should now be gone

<img width="530" height="288" alt="image" src="https://github.com/user-attachments/assets/0fb84598-fc27-4809-890c-36448fb74df3" />

Once you refresh the Billing and Cost Management page on the user account you will now be able to see your data

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9e7e57e2-fec0-4589-90c9-5958bc8e36ad" />

