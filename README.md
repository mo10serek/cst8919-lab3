# CST8919 Lab 3

## Summary

There are 3 policies that we need to set up for this assignment. To make these policies is to go to the policy webpage in azure. Go to the **Definition** tab and make a policy by clicking **+ Policy definition**. Developed the json file that it will reject the resource validation if it violate the rules.

After that, we need to group these policies by making a Policy Initiative. To make a Initiative is to click **+ Initiative definition** in the **Definition** tab and add each of the policies you made to the group.

After that, go to assignment tab and click **Assign initiative** to assign the initiative you made.

To test the policies you made, try make a virtual machine in East US region, make a storage account without a `ProjectName` tag, and make a public IP resource.  If the validation had failed, then the policies worked. Also try to make a virtual machine in Canada Central with a tag to see if got accepted.

## Explanation of each policy

First, we need to set up a policy that a resource is only available in Central Canada. The second policy that we need to have a policy that a resource must have a `ProjectName` tag. The third policy is that a public Ip resource cannot be made. 

## Challenges and lessons learned

The lesson I leaned in this lab is making polices in json format, make an initiative and group each policy together, and also assigning an initiative to a group. 

## Demo

[demo](https://youtu.be/5fDaapAJCRc)