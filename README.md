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
A policy will be created to block access to EC2 management for the newlyt attached account. The policies are navigated and Service control policies is clicked. Enabled is selected:<br/>
<img src="https://imagizer.imageshack.com/img922/7681/8pEYYL.png" alt="Disk Sanitization Steps"/>
<br />
<br />
:<br/>
<img src="https://imagizer.imageshack.com/img922/8844/eYW7ao.png" alt="Disk Sanitization Steps"/>
<br />
<br />
:<br/>
<img src="https://imagizer.imageshack.com/img922/3706/oOCKof.png" alt="Disk Sanitization Steps"/>
<br />
<br />
:<br/>
<img src="https://imagizer.imageshack.com/img922/970/3Ymmio.png" alt="Disk Sanitization Steps"/>
<br />
<br />
:<br/>
<img src="https://imagizer.imageshack.com/img924/9946/qY0IJ6.png" alt="Disk Sanitization Steps"/>
<br />
<br />
:<br/>
<img src="https://imagizer.imageshack.com/img922/4418/lIz6YZ.png" alt="Disk Sanitization Steps"/>
<br />
<br />
:<br/>
<img src="https://imagizer.imageshack.com/img924/630/3M1hFd.png" alt="Disk Sanitization Steps"/>
<br />
<br />
:<br/>
<img src="https://imagizer.imageshack.com/img923/6273/B6O1bg.png" alt="Disk Sanitization Steps"/>
<br />
<br />
:<br/>
<img src="https://imagizer.imageshack.com/img924/5151/8u2fie.png" alt="Disk Sanitization Steps"/>
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
