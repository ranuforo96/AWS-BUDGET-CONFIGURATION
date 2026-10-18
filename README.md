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

<img width="567" height="619" alt="image" src="https://github.com/user-attachments/assets/c0d35660-3005-4ccb-b8dd-71189504c7c5" />

If you scroll down further, you can see the total number of active services. I currently have 9 services

<img width="1541" height="723" alt="image" src="https://github.com/user-attachments/assets/c1b7a53d-7019-44ac-bc60-32cd64418f07" />

For instance, clicking on Amazon Elastic Compute Cloud (EC2) allows you to view the exact costs and a detailed expense breakdown

<img width="1465" height="669" alt="image" src="https://github.com/user-attachments/assets/f9da4a04-efcf-4352-af44-25ddfc1d9290" />

Use the Free Tier dashboard in the left navigation menu to monitor current and forecasted usage, ensuring you don't exceed your free limits and incur charges

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e7497661-8064-4bee-9170-71881318fe11" />

<img width="1492" height="582" alt="image" src="https://github.com/user-attachments/assets/b320bdd9-f050-4f8a-b361-0b65b9286bf3" />

<img width="1499" height="579" alt="image" src="https://github.com/user-attachments/assets/39d4a68c-5a53-4180-b2e7-33bb0c126d66" />

Now we can set up a budget. On the left-hand side, scroll down until you see "Budgets and Planning" and select Budgets underneath it

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/010ba14b-5db0-417c-9565-c46678396d07" />

Here you can set custom thresholds that alert you when you exceed your budgeted thresholds

We start by right-clicking "Create a budget"

<img width="1316" height="384" alt="image" src="https://github.com/user-attachments/assets/3a93cf4f-6c9a-4703-9af9-e37ff4797f5f" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b2c883f1-c3e6-4073-b1cb-bd8468a2bb6d" />

Once the page has loaded, you can keep the simplified template checked

<img width="534" height="294" alt="image" src="https://github.com/user-attachments/assets/28e25749-0b38-4970-b5bb-23135219e8d2" />

And the first budget we will create will be a Zero spend budget, so that can also stay checked

This budget triggers an alert when your spending exceeds 1 cent

<img width="517" height="516" alt="image" src="https://github.com/user-attachments/assets/7388cdb7-2ea2-4590-9a80-48e5c790b4ae" />

The budget name will be "My Zero-Spend Budget"

Then, in the Email recipients box, enter the email address of the recipients you want to receive the alerts

<img width="527" height="522" alt="image" src="https://github.com/user-attachments/assets/6cc50b6a-8b4b-4d3c-aa7e-27335734975b" />

Once the information is entered, you can proceed with the budget creation by clicking "Create budget"

<img width="564" height="550" alt="image" src="https://github.com/user-attachments/assets/ef2df6ef-3b3d-4dfa-b465-b29100f73e20" />

The budget should now be successfully created

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4a6edcaa-ae45-4cf1-8d20-6d5693beed9b" />

However, if we want to create a monthly cost budget, we can also use the same simplified template and make sure you check the Monthly cost budget under templates

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8039ef32-bf1a-4095-8a65-ff5494a56fc6" />

For this example, I don't want to exceed 12 dollars for the month, so to give this a descriptive name, I will be naming this budget "My Monthly Cost Budget ($12)"

As for the budget amount, I will enter 12 into the prompt, enter my email in the recipient box, and click Create budget to finalize the creation

This budget will actually alert 3 times: 1. "your actual spend reaches 85%", 2. "your actual spend reaches 100%", and  3. "if your forecasted spend is expected to reach 100%"

<img width="1007" height="428" alt="image" src="https://github.com/user-attachments/assets/04b9efef-3f56-4ca3-9ac2-0415e7c466c8" />

<img width="391" height="315" alt="image" src="https://github.com/user-attachments/assets/4e1c4c6f-78ad-4733-b2f9-20b16ffb7a0b" />

The budget should now be successfully created: 

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/951f0325-007f-4568-a972-f67a2ba120c3" />
