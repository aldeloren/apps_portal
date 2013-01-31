# Installation of apps.ufl.edu customizations.

## Files
All files needed for installation are contained within this repo. There will also be some pre-existing files that need to be modified included with the XenApp install.

## Install new files:
The repo follows the XenApp's folder structure.


Move the included inetpub/wwwroot/XenApp/media/custom folder into the servers referenced media folder.

Replace the pre-existing `footer.inc` file with the included `inetpub/wwwroot/XenApp/app_data/include/footer.inc` .

Append the pre-existing `fullstyle.inc` file with the included `inetpub/wwwroot/XenApp/app_data/include/fullstyle.inc` .

## Modify existing files:
Edit as outlined below

C\Program Files (x86)\Citrix\Web Interface\5.4.0\languages\accessplatform_strings.properties:

line 157:
`UserName=Gatorlink ID:`

line 167:
`BlankUsername=You must enter a valid Gatorlink ID.`

line 176:
`GeneralCredentialsFailure=Please verify your Gatorlink ID and password and try logging on again. If you cannot log on, contact your help desk.`


C\Program Files (x86)\Citrix\Web Interface\5.4.0\languages\common_strings.properties:

line 231:
`NoUsername=You must specify a valid Gatorlink ID.`

## Modify through Web interface
Citrix WebApp Interface Management -> Web Site Appearance -> Appearance -> Header Area:

Change both Full Graphics Mode and Low graphics mode to:
`../media/custom/appslogo.png`
