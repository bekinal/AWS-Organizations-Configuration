<h1>AWS Organizations Configuration</h1>

<h2>Description</h2>
Project consists of creating AWS organizations to allow centralized management for multiple AWS accounts
<br />


<h2>Utilities Used</h2>

- <b>Amazon Web Services</b>

<h2>Creating an AWS Organization:</h2>
An AWS organization will be created, and access will be granted to its management console and features. To do this, AWS orgnizations is navigated to:<br/>
<img src="https://imagizer.imageshack.com/img924/7366/zKzy7C.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Create an organization is selected. This organization is created with the root user and a management account:<br/>
<img src="https://imagizer.imageshack.com/img923/1116/PSNVxJ.png" alt="Disk Sanitization Steps"/>
<br />
<br />
 Clicking Add an AWS account will add a new account to the organization:<br/>
<img src="https://imagizer.imageshack.com/img924/7493/gTpBcv.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Create an AWS account is selected:<br/>
<img src="https://imagizer.imageshack.com/img923/5300/M9qWr9.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The accounts credentials are defined. This email must not already be used within the AWS account:<br/>
<img src="https://imagizer.imageshack.com/img924/4852/ozC01N.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The new account is active as it appears in the AWS Organization:<br/>
<img src="https://imagizer.imageshack.com/img922/4/erfx3f.png" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>Creating a Policy:</h2>
A policy will be created to block access to EC2 management for the newly attached account. The policies are navigated and Service control policies is clicked. Enabled is selected:<br/>
<img src="https://imagizer.imageshack.com/img922/7681/8pEYYL.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Enable service control policies is selected:<br/>
<img src="https://imagizer.imageshack.com/img922/8844/eYW7ao.png" alt="Disk Sanitization Steps"/>
<br />
<br />
After noting that the service control policies are enabled, Create policy is selcted:<br/>
<img src="https://imagizer.imageshack.com/img922/3706/oOCKof.png" alt="Disk Sanitization Steps"/>
<br />
<br />
the policy is named EC2 Deny Management and a short desciption is provided:<br/>
<img src="https://imagizer.imageshack.com/img922/970/3Ymmio.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Ec2 is selected, and All actions is checked. The Effect should be deny:<br/>
<img src="https://imagizer.imageshack.com/img924/9946/qY0IJ6.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Add a resource is selected:<br/>
<img src="https://imagizer.imageshack.com/img922/4418/lIz6YZ.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The EC2 service is selected. Resource type is set to all. Add resource is clicked:<br/>
<img src="https://imagizer.imageshack.com/img924/630/3M1hFd.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Create policy is selected:<br/>
<img src="https://imagizer.imageshack.com/img923/6273/B6O1bg.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The new policy can be viewed in the dashboard:<br/>
<img src="https://imagizer.imageshack.com/img924/5151/8u2fie.png" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>Policy attachment and verification:</h2>
The EC2 Deny Management policy is selected:<br/>
<img src="https://imagizer.imageshack.com/img924/4197/SXeUcK.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The actions dropdown menu is clicked to select Attach policy:<br/>
<img src="https://imagizer.imageshack.com/img924/8107/S2lKXI.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The nicknamed account is selected and the polciy is attached:<br/>
<img src="https://imagizer.imageshack.com/img923/9901/bH1Wo1.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The root account is signed out:<br/>
<img src="https://imagizer.imageshack.com/img923/7093/FYLsDm.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The nicknamed account will now be attempted to sign in:<br/>
<img src="https://imagizer.imageshack.com/img922/9711/mB67Qh.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Upon initial login, forgot password is selected:<br/>
<img src="https://imagizer.imageshack.com/img923/9332/2FtkOP.png" alt="Disk Sanitization Steps"/>
<br />
<br />
A message is sent to the attached email of the account:<br/>
<img src="https://imagizer.imageshack.com/img923/5634/IlCZea.png" alt="Disk Sanitization Steps"/>
<br />
<br />
A new password is then created:<br/>
<img src="https://imagizer.imageshack.com/img922/1098/oRawsG.png" alt="Disk Sanitization Steps"/>
<br />
<br />
At the AWS console home, EC2 is selected:<br/>
<img src="https://imagizer.imageshack.com/img923/4967/a2u1pc.png" alt="Disk Sanitization Steps"/>
<br />
<br />
It can be noted that all APIs are errored out. Attempting to launch an EC2 instance will provide a message specifying that I am not authorized to perform this operation:<br/>
<img src="https://imagizer.imageshack.com/img923/8875/OeddET.png" alt="Disk Sanitization Steps"/>
<br />
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
