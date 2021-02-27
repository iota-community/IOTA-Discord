This guide explains how to get issues from GitHub into the IOTA Experience Team channels.
Every IOTA Experience Team Initiative is assigned a GitHub repository in the iota-community group. It is possible to set up webhooks, to cross-communicate initiatives and events from GitHub to Discord.
*example*:
![img](/_resources/images/settings/aca05222-5d18-4b08-ac42-232cbaacb4c4.PNG)
## Instructions
In **this example** we will set up the webhook for the **IOTA Streams Experience Team**.
1. Go to the X-Team relative channel in Discord and **Edit the channel**  
   ![img](/_resources/images/settings/5b500455-12b4-43e9-9a2c-0c9e0dfa3e6d.png)
2. Click on **Webhooks** on the left side and then on the **Create Webhook** button on the right side  
   ![img](/_resources/images/settings/3d34b740-28ad-4879-b2ff-e0f38cba9f37.png)
3. Change the name to **GitHub**, click on the **Copy** button to copy the webhook link and click on the **Save** button, to save this settings.  
   *(e.g. of this webhook link:* [*https://discordapp.com/api/webhooks/704234568231682099/oo_wo_qWi-FJXSRnedRvZ0yoDuhkn7MjZPQ5njtHcy3SQIWCqrXOmRDhBxjGHrqWBAou*](https://discordapp.com/api/webhooks/704234568231682099/oo_wo_qWi-FJXSRnedRvZ0yoDuhkn7MjZPQ5njtHcy3SQIWCqrXOmRDhBxjGHrqWBAou)*)*
   ![img](/_resources/images/settings/9f06b278-0540-46b6-b972-287c3d529c0a.png)
4. Now we go to the IOTA Experience Team - IOTA Streams GitHub repository  
   [iota-community/X-Team_IOTA_Streams](https://github.com/iota-community/iotastreams) 
5. Here we click on **Settings**, then **Webhooks** and finally the **Add webhook** button  
   ![img](/_resources/images/settings/33ce7b26-2443-42f8-91c6-341cd6ff0b24.png)
6. Insert your password to confirm  
   ![img](/_resources/images/settings/8acc22c2-fef1-4294-8e72-08e6e519e7b0.png)
7. In the **Payload URL** field we insert the **webhook link** we copied **from Discord** and **add /github** at the end.
   If the link was:
   https://discordapp.com/api/webhooks/704234568231682099/oo_wo_qWi-FJXSRnedRvZ0yoDuhkn7MjZPQ5njtHcy3SQIWCqrXOmRDhBxjGHrqWBAou  
   Now it is:  
   https://discordapp.com/api/webhooks/704234568231682099/oo_wo_qWi-FJXSRnedRvZ0yoDuhkn7MjZPQ5njtHcy3SQIWCqrXOmRDhBxjGHrqWBAou/github    
   and we **change** the **Content type** to **application/json**.  
   ![img](/_resources/images/settings/d1f5f1f3-13c6-4295-a8d6-6cdcfa3edd91.png)
8. In the **Which events would you like to trigger this webhook** section, chose **Let me select individual events**.  
   Now **select** the events that will be **posted to Discord**, adjust accordingly or through experience.  

   In this example we have:
   \- Issue comments
   \- Issues
   \- Collaborator add, remove, or changed
   \- Milestones
   \- Pushes

   Make sure the **webhook** is **active** and finally press the **Add webhook** button.  
   ![img](/_resources/images/settings/1e4936e3-2899-4f93-bfcd-c948aef84fb6.png)
9. As you click on the **Add webook**, the GitHub page will show a notification at the top and a **green checkmark** to show that the settings are correct.  
   ![img](/_resources/images/settings/a4e44e68-b493-4db4-87dc-852a3ed0407e.png)
