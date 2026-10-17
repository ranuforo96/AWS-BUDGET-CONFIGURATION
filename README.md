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

Once you refresh the Billing and Cost Management page on the user account, you will now be able to see your Cost summary data except for "Total forecasted cost for current month", because there is not enough historical data to forecast

Cost summary gives you a high-level overview of your spending, showing metrics like your month-to-date costs, comparisons to last month, and forecasted spending

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9e7e57e2-fec0-4589-90c9-5958bc8e36ad" />

<img width="736" height="219" alt="image" src="https://github.com/user-attachments/assets/4056da2c-bc3a-4161-a8b5-2c04ac90524c" />

The cost breakdown, on the other hand, complements this by displaying exactly which services are driving those costs, such as EC2 or S3, giving you a clearer view of your service-level monthly spending, which can be seen in the screenshot below

<img width="742" height="574" alt="image" src="https://github.com/user-attachments/assets/3006b972-55ed-405b-b271-3a9fddd60c5b" />

Then, in the left navigation pane, if you select Bills, this is your primary dashboard for monitoring your current spending and charges within a specific billing period

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/22ad27db-05a9-41d1-8648-b3aec8295814" />

If you scroll down further, you can see the total number of active services. I currently have 9 services

<img width="1541" height="723" alt="image" src="https://github.com/user-attachments/assets/c1b7a53d-7019-44ac-bc60-32cd64418f07" />

For instance, clicking on Amazon Elastic Compute Cloud (EC2) allows you to view the exact costs and a detailed expense breakdown

<img width="1465" height="669" alt="image" src="https://github.com/user-attachments/assets/f9da4a04-efcf-4352-af44-25ddfc1d9290" />

