# YUNOHOST user, application, and system account management best practice: vision and tools

*This present document is to help large community members, administrators and managers to manage YUNOHOST access rights through a good understanding of the right access management and with the help of a visual tool.* 

*Please, note at the time this vision has been written, there is no access group strategy in YUNOHOST. This is not an obstacle.*

**Status: to be developed**

## Role management in YUNOHOST
From this YNH page: [Overview of the YUNOHOST ecosystem](https://yunohost.org/#/overview_en),
this sketch which give you a first idea of the accounts management (even if this sketch has a larger topic)

![access right in YUNOHOST](/images/ecosystem[1].png)

## Access right levels in YUNOHOST
The list below takes account of the (1)application administration and (2) the administration of the hardware/VPS where the YNH has been installed.

Extended list of access rights in YUNOHOST:
1. Visitor, 
2. YNH user,
3. YNH application user/admin (not declared in YNH but in the application (e.g. Wordpress, Next Cloud)
4. YNH Application administrator (declared in the YNH application during the installation process)
5. YNH superuser (the first user)
5. YUNOHOST administrator
6. Root admin (Debian serveur)
7. Hardware/VPS host admin administrator

Even if some of these access rights are held by the same user, for instance, the three last, this must be very clear for all the organization.
Here, the "YNH application administrator" has been differentiated from a "basic user" as this account could be a generic account (not recommended).

## Role in the organization
To establish the best access right policy, it is very important to have a good understanding of the organization and its actors.

The list is an example of an organization 

YNH Role   | YNH applications |  Role in organization  |   Access right
---------------|-----------|------------------------|-----------------
Visitor (members or non-members) | Website, forum (no-connected)   | Users, fans, members as visitor | Applications with a Public status
YNH user | Email, set of dedicated applications for members | At least member | Given through YNH attribution 
YNH user with a special right given by YNH applications | Forum Moderator, WP admin, redactor, contributor... | In charge or member of a dedicated committee or working group| Given through application attribution (example WordPress)  |  
YNH admin | YNH administration | Depend on the organization | YNH top-level access right 
Root admin | YNH server | Depend on the organization | Can delete or make inaccessible YNH 
Hardware admin | Power on/off the server | Depend on the organization | Can power off the server 

From the list below, the access right management can be defined through a tool like this list below (Calc).
* Please, take into consideration the framework, not its content. For instance, the president of the organization can have all the top-level access right or not, it depends on its "technical legitimacy" or how he sees its role. Or how he trusts its administrator.*

![Example. Tool for access right management in a large community](/images/Screen-Copy_access-right_20190806.JPG)

Even if this file, in its first issue, has not a great value, you can download it from here : ![Example. Calc file for YNH account management v0.1](/files/YNH-Access-right-management-tool_v0.1.ods)

Next step :
- [ ] to be discussed
- [ ] to be reviewed under a review of all existing YNH access right functions

Thank you for your contribution.
Please note I am not at ease with GitHub. If you think your comment does not reach me, contact me through the YUNOHOST forum: https://forum.yunohost.org/.

JRelland. jrd or José
Update, 20190811, from an exchange with ljf at the YNH camp 2019
Creation, 2019/08/06


