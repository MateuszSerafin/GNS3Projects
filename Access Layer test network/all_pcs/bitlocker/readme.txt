I have found out that there are multiple ways to setup bitlocker.
Network unlock would be good in my case however I am using dot1x and it would not be able to communicate with domain controller this means it would not work, also adding exceptions such as those is weird not sure how real deployment of that would look like
PIN, pin would maybe be good however there are issues with it. This would basically mean that the pin would need to be shared amongst employees which means literary someone could share it and point of encryption is somewhat useless in that case
TPM the best way i see it to use TPM. Someone could steal the hard-drive but it would be encrypted as those PC's would be inside company someone would need to steal whole PC in order to access TPM and after it's still sophisticated attack.

Also look at GPO's from DC0 for configuration of that

It looks like that there is an option -AdAccountOrGroupProtector. I am currently testing it's behaviour
but from what i have seen it uses tpm,Numerical password and Identity of user.
This would be ideal because if it would encrypt just base of windows (it wouldn't really matter if someone would steal it).
And then encrypt each user data differently based on a password it would be what i need for this network.
Unfortunately testing this takes time