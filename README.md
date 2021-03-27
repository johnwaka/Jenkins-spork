# Jenkins-spork
### Failed to connect to repository” Error while setting up Github Jenkins Plugin
This article shows how to fix "failed to connect to repository” Error while setting up Github Jenkins Plugin.


![image](https://user-images.githubusercontent.com/11300636/112729754-d1785280-8f3e-11eb-93b6-58896797c33a.png)


You might get this error when you try to paste a repository URL in the "Source Code Management > Git > Repository URL" section of a new job in Jenkins.
The problem may occur when your system cannot locate git installation. You need to make sure you have git installed in your system. A simple way to check in Windows is as shown below:


![image](https://user-images.githubusercontent.com/11300636/112729704-96761f00-8f3e-11eb-87d9-4e89ab33b935.png)
 

Once you have verified you have git installed. If you are using Jenkins on a VM or local system, locate the git installation folder. A simple way to get this location is running a PowerShell command.

![image](https://user-images.githubusercontent.com/11300636/112729784-01bff100-8f3f-11eb-8a24-7c6c44bfb1f9.png)

Once you have the path, you need to set the path to your git executable in Manage Jenkins -> Global Tool Configuration -> Git -> Git Installations -> Path to Git executable.

![image](https://user-images.githubusercontent.com/11300636/112729886-87dc3780-8f3f-11eb-8ae3-b6d7b0477f21.png)


 
After this you can paste your repository URL and it will not give any errors:

![image](https://user-images.githubusercontent.com/11300636/112729787-0c7a8600-8f3f-11eb-9aef-e44944f98bd2.png)

 
