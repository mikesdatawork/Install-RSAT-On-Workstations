![MIKES DATA WORK GIT REPO](https://raw.githubusercontent.com/mikesdatawork/images/master/git_mikes_data_work_banner_01.png "Mikes Data Work")        

# Install RSAT On Workstations
**Post Date: June 4, 2015**        



## Contents    
- [About Process](##About-Process)  
- [Author](#Author)  
- [License](#License)       

## About-Process

<p>So; you're a DBA trying to configure something in the database system, and so it's pretty ordinary stuff that you'll need to browse Active Directory to find Shares, Accounts, Groups, OU's, Members etc. You'll need to turn the Remote Server Administration Tools on so you can get to dsa.msc. However; when you go to the features you see they are missing. Now you have to install it, and then add the feature. Here's some quick steps to help you with that process.</p>

Get the .msu file and install it using these super easy steps.
1.	Download RSAT:https://www.microsoft.com/en-us/download/details.aspx?id=7887
2.	Copy it to root of  C:
3.	Run it from command prompt (open the command prompts as administrator or with admin account)
4.	Paste this, and run it:  wusa C:Windows6.1-KB958830-x64-RefreshPkg.msu

Just click through the prompts when the installation starts. Takes about 5 minutes.

![Run WUSA Command]( https://mikesdatawork.files.wordpress.com/2015/06/image003.jpg "Run WUSA Command")
 
Next you'll want to add the feature just as before.
Go to Start Run: appwiz.cpl
![Run AppWiz]( https://mikesdatawork.files.wordpress.com/2015/06/image004.jpg "Run AppWiz")
 
Select 'Turn Windows Features on or off'.

![Turn Windows Features On]( https://mikesdatawork.files.wordpress.com/2015/06/image005.jpg "Turn Windows Features On")
 
Select the following features, and click next through the prompts to have them installed.
•	Remote Server Administration Tools
•	Role Administration Tools
•	AD DS and AD LDS Tools
•	Active Directory Administrative Center
•	AD DS Snap-ins and Command-line Tools
•	Server NIS Tools
•	Remote Server Desktop Tools
![Turn Features On]( https://mikesdatawork.files.wordpress.com/2015/06/image006.jpg "Turn Windows Features On")
 


[![WorksEveryTime](https://forthebadge.com/images/badges/60-percent-of-the-time-works-every-time.svg)](https://shitday.de/)

## Author

[![Gist](https://img.shields.io/badge/Gist-MikesDataWork-<COLOR>.svg)](https://gist.github.com/mikesdatawork)
[![Twitter](https://img.shields.io/badge/Twitter-MikesDataWork-<COLOR>.svg)](https://twitter.com/mikesdatawork)
[![Wordpress](https://img.shields.io/badge/Wordpress-MikesDataWork-<COLOR>.svg)](https://mikesdatawork.wordpress.com/)

    
## License
[![LicenseCCSA](https://img.shields.io/badge/License-CreativeCommonsSA-<COLOR>.svg)](https://creativecommons.org/share-your-work/licensing-types-examples/)

![Mikes Data Work](https://raw.githubusercontent.com/mikesdatawork/images/master/git_mikes_data_work_banner_02.png "Mikes Data Work")

