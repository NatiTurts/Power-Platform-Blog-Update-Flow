# Power Platform Blog Update Flow


## Summary

Having multiple RSS flows per Power Platform product can get messy. More over, it's not always user friendly accessing these updates through the Power Automate notifications. These two flows, a weekly and daily flow, retrieve all Power Platform product blog updates and summarize them into product categories through a neat HTML template. Then once a week/day, users can receive a summary of all blog updates via email with links to each individual blog post.

![picture of the flow](assets/images/Flow.gif)

## Applies to

* [Microsoft Power Automate](https://docs.microsoft.com/power-automate)

## Compatibility

![Premium License](https://img.shields.io/badge/Premium%20License-Not%20Required-green.svg "Premium license not required")
![On-Premises Connectors](https://img.shields.io/badge/On--Premises%20Connectors-No-green.svg "Does not use on-premise connectors")
![Custom Connectors](https://img.shields.io/badge/Custom%20Connectors-Not%20Required-green.svg "Does not use custom connectors")

## Authors

Solution|Author(s)
--------|---------
Power Platform Blog Update Flow | [Nati Turtledove](https://github.com/NatiTurts) ([@NatiTurts](https://www.twitter.com/NatiTurts) )

## Version history

Version|Date|Comments
-------|----|--------
1.0.0.0  |March 24, 2023|Initial release

## Features

* Scheduled: two flows for both weekly and daily email updates. 
* RSS Feed: Consolidated all Power Platform RSS Feed blog updates.
* HTML Template: Blog updates are wrapped in an elegant customizable HTML template that is delivered via email

## Setup

### Environment Variable
When importing the solution, add your email, or a designated group email into the variable. This varibale is used for the `To` in the Office 365 Outlook connector. This is the address the flow will send the updates to.

### Updating the Variables
The flows consist of various variables that contain base64 image files and other header and footer text. Below are a list of variables that should be updated. 
* varGitHubAddress
* varYouTubeAddress
* varTwitterAddress
* varLinkedInAddress
* varWebsite
* varLinkedInIcon
* varYouTubeIcon
* varTwitterIcon
* varGithubIconvarHeader
* varEmailSubject
* varFooter
* varLogo

Note that all icon and image variables need to contain the base64 image text. To convert your images to base64, I recommend you use the base64-image website, https://www.base64-image.de/



## Minimal Path to Awesome

* [Download](solution/Power-Platform-Blog-Update-Flow.zip) the `.zip` from the `solution` folder
* [Import](https://flow.microsoft.com/en-us/blog/import-export-bap-packages/) the `.zip` file using **My Flows** > **Import** > **Upload** within Microsoft Flow.

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**


## Help

We do not support samples, but we this community is always willing to help, and we want to improve these samples. We use GitHub to track issues, which makes it easy for  community members to volunteer their time and help resolve issues.

If you encounter any issues while using this sample, [create a new issue](https://github.com/pnp/powerautomate-samples/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=bug-report.yml&sample=Power-Platform-Blog-Update-Flow&authors=@NatiTurts&title=Power-Platform-Blog-Update-Flow%20-%20).

For questions regarding this sample, [create a new question](https://github.com/pnp/powerautomate-samples/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=question.yml&sample=Power-Platform-Blog-Update-Flow&authors=@NatiTurts&title=Power-Platform-Blog-Update-Flow%20-%20).

Finally, if you have an idea for improvement, [make a suggestion](https://github.com/pnp/powerautomate-samples/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=suggestion.yml&sample=Power-Platform-Blog-Update-Flow&authors=@NatiTurts&title=Power-Platform-Blog-Update-Flow%20-%20).

## For more information

- [Create your first flow](https://docs.microsoft.com/en-us/power-automate/getting-started#create-your-first-flow)
- [Microsoft Power Automate documentation](https://docs.microsoft.com/en-us/power-automate/)

<img src="https://telemetry.sharepointpnp.com/powerautomate-samples/samples/Power-Platform-Blog-Update-Flow" />
