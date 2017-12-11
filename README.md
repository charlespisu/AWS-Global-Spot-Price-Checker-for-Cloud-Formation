# AWS-Global-Spot-Price-Checker-for-Cloud-Formation
Will tell you the lowest priced region and AZ for each Instance Type you pick in the parameters section.  Outputs can be read in instance logs saving you the need to connect to an instnace or manually run any commands.

# Steps to run:
1) Download locally
2) Creae Stack in CloudFormation and choose to Upload a template to Amazon S3, select SpotPrice.template from this download.
3)  Name the stack, provide a Key Pair from the dropdown, select the instance types you want to see the  spot prices for
4) Skip Options Screen
5) On Review screen Acknowledge that AWS CloudFormation might create IAM Resources,
6) Create, wait 2 minutes, then go to EC2, click on instance, and in the top bar select Actions -> Instance Settings -> Get System Log -> Scroll to bottom to see each Instance's spot price for all regions and cheapest spot price globally.

Example Output:
</br>
![Alt text](https://github.com/charlespisu/AWS-Global-Spot-Price-Checker-for-Cloud-Formation/blob/master/Capture.PNG "Example Spot Price Checker Output")
