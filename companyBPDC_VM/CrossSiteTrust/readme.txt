1. Setup conditional forwarder 

2. Trust other domain. In my case i did selective trust. In GUI this is just point and click. Really not hard.
But when you want to actaully login to this user some steps involved.

3. CompanyA has universal group i want to allow login. So i just created a group that overall allows logging from other domains. (Domain Local)

4. Then you need to go to machine that you want to allow access to login and using advanced features view go to security prooperties and add this domain local group. Other wise it will error with firewall authentication or something like that
