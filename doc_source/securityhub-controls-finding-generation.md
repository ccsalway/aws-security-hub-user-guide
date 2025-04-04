# How AWS Security Hub runs and uses security checks<a name="securityhub-controls-finding-generation"></a>

For each enabled control, AWS Security Hub runs security checks\. A security check determines whether your resources are in compliance with the control requirements\.

Some checks run on a regular schedule\. Other checks only run when there is a change to the resource state\. See [Schedule for running security checks](securityhub-standards-schedule.md)\.

Many security checks use AWS Config managed or custom rules to establish the compliance requirements\. To run these checks, you must have AWS Config enabled\. See [How Security Hub uses AWS Config rules to run security checks](securityhub-standards-awsconfigrules.md)\. Others use custom Lambda functions, which are managed by Security Hub and are not visible to customers\.

For each check, Security Hub creates or updates a finding\. See [Generating and updating control findings](controls-findings-create-update.md)\.

Security Hub uses the findings to assess your security posture for each control and across an entire standard\. See [Determining the overall status of a control from its findings](controls-overall-status.md) and [Determining the security score for a security standard](standards-security-score.md)\.

**Topics**
+ [How Security Hub uses AWS Config rules to run security checks](securityhub-standards-awsconfigrules.md)
+ [Schedule for running security checks](securityhub-standards-schedule.md)
+ [Generating and updating control findings](controls-findings-create-update.md)
+ [Determining the overall status of a control from its findings](controls-overall-status.md)
+ [Determining the security score for a security standard](standards-security-score.md)