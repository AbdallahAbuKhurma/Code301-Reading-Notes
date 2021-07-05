# Access Control (ACL)
>
## When is basic authorization used v. bearer authorization

Basic authorization is used to authenticate a user (grab authorization header, extract components, autheticate). Bearer Authorization is validating that a user has the correct token to proceed in the route, bearer authorization we are authenticating the token.

## What does the JSON web token package do

Creates a token based off of a users hashed username from the database + the app SECRET.

## What considerations should we make when creating and storing a SECRET

Storing the secret someplace secure, (.env files are good) and storing secrets with some level of encryption.

## Terminology

* Encryption:

  * translates/hashes data into a different form that is difficult to crack to ensure the security of important data

* Token:

  * piece of data needed to access otherwise restricted areas of an application

* Bearer:

  * person/thing that carries or holds bad news

  * pertaining to programming, refers to a user having a piece of required data which then grants authorization to elements not available to most users

* Secret:

  * a keyword within the app itself that is used toward authentication

* JSON Web Token:

  * a node package that allows us to create and verify ‘tokens’

* Authorization Code:

  * temporary code or authorization that exchanges for an access token

  * obtained from authorization route/endpoint

* Access Token:

  * used in token based authentication which allows access to other routes/data that are otherwise restricted

## RBAC

* Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges.ِand the idea of assigning system access to users based on their role within an organization.

* When using RBAC, you analyze the needs of your users and group them into roles based on common responsibilities.You then assign one or more roles to each user and one or more permissions to each role. The user-role and role-permissions relationships make it simple to perform user assignments since users no longer need to be managed individually, but instead have privileges that conform to the permissions assigned to their role(s).

## 5 steps to RBAC

1. ***Inventory your systems:*** Figure out what resources you have for which you need to control access, if you don't already have them listed. Examples would include an email system, customer database, contact management system, major folders on a file server, etc.

2. ***Analyze your workforce and create roles:*** You need to group your workforce members into roles with common access needs. Avoid the temptation to have too many roles defined. Keep them as simple and stratified as possible.

3. ***Assign people to roles:*** Now that you have a list of roles and their access rights, figure out which role(s) each employee belongs in, and set their access accordingly.

4. ***Never make one-off changes:*** Resist any temptation to make a one-off change for an employee with unusual needs. If you begin doing this, your RBAC system will quickly begin to unravel. Change the roles as required or add new ones when really necessary.

5. ***Audit:*** Periodically review your roles, the employees assigned to them, and the access permitted for each. If you discover, for example, that a role has unnecessary access to a particular system, change the role and adjust the access level for all employees in that role.

## Resources

[RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)

[5 steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

[wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)
