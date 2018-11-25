# Chapter 03: Identity and Access Management (IAM)

## IAM 101

* IAM allows you to manage users and their access to the AWS console
    * Shared access (also temporary) to your account
    * Supports multifactor authentication (MFA)
    * Supports identity federation (e.g. AD, Facebook, etc.)
    * Supports granting granular permissions
    * Supports defining password rotation strategies
* Terminology:
    * Users: End users
    * Groups: An array of users under one set of permissions
    * Roles: Can be assigned to AWS resources
    * Policies: A document that defines one or more permissions

## IAM Lab

* IAM does not support regions - it is a global service
* You should always enable MFA
* You should create new users instead of using root account all the time
    * Make sure user has both programmatic and console access
    * Assign user to a group and grant policies to this group
    * Root account has been granted 'AdministratorAccess' policies
    * Policies can apparently be added to groups and users
    * The following user information is created
        * **Access key id** and **Secret access key** for programmatic access
        * **Password** for access to the AWS console
        * You will only see these credentials once, later on you can **inactivate** them and generate new credentials 

