# Access Control (ACL)
![API](https://nordicapis.com/wp-content/uploads/Building-a-RESTful-API-Using-Node.JS-and-MongoDB.png)

1. When is Basic Authorization used vs. Bearer Authorization?

he Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret (see RFC7616 and RFC7617). The Bearer authentication scheme is dedicated to the authentication using a token and is described by the RFC6750.

2. What does the JSON Web Token package do?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

3. What considerations should we make when creating and storing a SECRET?

don’t create a weak secret.
don’t store it in a plain text.
don’t share your secret with anyone.

* RBAC tutorial

RBAC stands for Role Based Access Control and it is process by which we give permission to the user based on their access rights.
In some other words, It lets employees have access rights only to the information they need to do their jobs and prevents them from accessing information that doesn’t pertain to them.
You can take the example of the Indian Air Force, in which each officer has its own privileges. Based on that Government provide them (and families ) the facilities and accommodations etc.

* 5 steps to RBAC

1. nventory your systems. Figure out what resources you have for which you need to control access, if you don't  already have them listed. ...
2. Analyze your workforce and create roles. ...
3. Assign people to roles. ...
4. Never make one-off changes. ...
5. Audit.

* wiki - RBAC

When defining an RBAC model, the following conventions are useful:

S = Subject = A person or automated agent
R = Role = Job function or title which defines an authority level
P = Permissions = An approval of a mode of access to a resource
SE = Session = A mapping involving S, R and/or P
SA = Subject Assignment
PA = Permission Assignment
RH = Partially ordered Role Hierarchy. RH can also be written: ≥ (The notation: x ≥ y means that x inherits the permissions of y.)
A subject can have multiple roles.
A role can have multiple subjects.
A role can have many permissions.
A permission can be assigned to many roles.
An operation can be assigned to many permissions.
A permission can be assigned to many operations.
A constraint places a restrictive rule on the potential inheritance of permissions from opposing roles, thus it can be used to achieve appropriate separation of duties. For example, the same person should not be allowed to both create a login account and to authorize the account creation.