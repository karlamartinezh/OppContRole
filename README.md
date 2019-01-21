# OppContRole
Salesforce - Update Opportunity Contact Role 

I was facing an issue with the Opportunity Contact Role object, because I wasn't able to work with this obj like another one, this one is kinda special. It has limitations. 

"One current limitation with Salesforce.com native Opportunities model is the inability to have a trigger on the Opportunity Contact Role object. Say you have built a custom Opportunity rollup  upon what/who the user selects in the Opportunity Contact Role area: how will you detect a live change in related Opportunity Contact Roles?

Here's a trick to detect such a change using Visualforce and native Opportunity layouts. It's really about having your code "know" (and possibly execute) every time a user visits a native Salesforce layout (regardless of the object.) Hence, we could call it an "On-View" trigger"

Create a VF page with the name oppContRolePage 
Add the VF inside the Opportunity Layout with 0 width and 0 height - this will work as a controller

then create Opphelper apex class which will have a future method in order to update Opp. Contact Roles

You should set the permissions to yours individuals users add the VF page. 

I took this idea from https://www.soliantconsulting.com/blog/view-triggers-salesforce it was really helpfull to me btw!

