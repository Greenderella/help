---
layout: article
title: User Types and Access Control
categories: [organizations]
featured: true
popular: false
tags: [user types, access control]
---

## User Types

When adding users to your Bitwarden Organization, you can grant certain levels of access by user type. Options include Owner, Admin, Manager and User. See further details below:

### User
- Most common user type
- Only have access to assigned collections
- Consumers of shared items in addition to their individual vault items
- Only work with items under collections they have been associated with
- Unable to create collections

### Manager
- Only administer a collection it is associated with by an Owner or Admin
- Access and manage assigned collections in an organization
- Create new collections and modify the assigned collections
- Able to set user access for assigned collections

### Admin
- Access and manage all items, collections, and users in your organization
- Invite and confirm users to join an organization
- Manage Enterprise Policies
- Manage Groups
- View Event Logs
- Export organization vault data
- Normally only a few select Admins in an organization

### Owner
- Highest level of access
- Manage all aspects of the organization
- Manage billing, subscription, and integration mechanisms
- Normally only a few select Owners in an organization

{% note %}
Once the user or user’s group is saved with their Collections access, the user will inherit those items into their Vault view.
{% endnote %}

## Access Control
In addition to defining the User Type, Access Control determines a full or partial view of the collections within an organization.

Choose **all items** or **selected collections** to set the appropriate access for the user.

{% note %}
Admin and Owner user-types can access all collections regardless of assignment when accessing Bitwarden from the Organization View. Assignments will control client access and display of collections.
{% endnote %}

### Item Access and Control

**Read Only**
- Selecting this option will prevent users assigned to this collection from adding new items, and editing or deleting existing items.

**Hide Passwords**
- This option hides passwords, TOTP seeds, and any custom fields of type *hidden* in this collection. This also disables the ability for an end-user to copy a password. In this configuration, an item may only be used with auto-fill.

{% warning %}
Enabling hidden passwords prevents the easy copy and paste of hidden items, however it does not completely prevent user access to this information. Please treat hidden passwords as you would any shared credential.
{% endwarning %}

{% image organizations/user-types-access-control.png %}
