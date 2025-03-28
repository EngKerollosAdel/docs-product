---
summary: Learn how OutSystems 11 (O11) manages application creation permissions, allowing architects to create applications while restricting junior developers.
locale: en-us
guid: f5ba93ec-ca75-43eb-a9ab-e0e83596927d
app_type: traditional web apps, mobile apps, reactive web apps
platform-version: o11
figma: https://www.figma.com/file/rEgQrcpdEWiKIORddoVydX/Managing%20the%20Applications%20Lifecycle?node-id=267:73
tags: application lifecycle management, permissions management, environment configuration, user roles, outsystems best practices
audience:
  - full stack developers
  - architects
outsystems-tools:
  - service studio
coverage-type:
  - apply
  - understand
---

# Control Who Creates Applications

OutSystems permission model allows you to limit the creation of new applications in an environment to some users, such as IT architects.

In this example we want to:

* Allow junior developers to see and work only on the applications of their respective teams but **without being able to create new applications**.

* Allow architects to **create applications** for their teams.

![Diagram illustrating the control of application creation within a team in OutSystems](images/control-app-creation-team-diag.png "Team Application Creation Control Diagram")

To do this, configure the junior developers:

1. [Create a new role](create-an-it-role.md#create-a-new-role) that has the permission level **Access**.  

    ![Screenshot showing the configuration of the junior developer access role in OutSystems](images/control-app-creation-junior-access-role-lt.png "Junior Developer Access Role Configuration")

1. [Create IT users](create-an-it-user.md) for all junior developers with this new role set as the default role. This defines base permissions that only allow all junior developers to log in to an environment without granting access to any application.

1. [Create another role](create-an-it-role.md#create-a-new-role) called Junior Developer that has the permission level **Change and Deploy Applications** and set the permission **Create Applications** to OFF.  

    ![Screenshot displaying the junior developer deploy role with create applications permission turned off in OutSystems](images/control-app-creation-junior-deploy-role-lt.png "Junior Developer Deploy Role Configuration")

1. [Add the junior developers to their respective teams](create-an-it-team.md#add-it-users-to-the-team) with the role Junior Developer. This allows junior developers to make changes to the existing applications in their teams but does not allow them to create new applications.

Then, configure the architects:

1. [Create a new role](create-an-it-role.md#create-a-new-role) called Architect that has the permission level **Change and Deploy Applications** and set the permission **Create Applications** to **ON**.  

    ![Screenshot of the architect role configuration with create applications permission enabled in OutSystems](images/control-app-creation-architect-role-lt.png "Architect Role Configuration")

2. [Add the architects to their respective teams](create-an-it-team.md#add-it-users-to-the-team) with the role Architect.  

    ![Screenshot depicting the process of adding an architect to a team in OutSystems](images/control-app-creation-add-architect-to-team-lt.png "Adding Architect to Team")

This allows architects to [create new applications directly in their teams](create-an-it-team.md#create-a-new-application-in-the-team) through LifeTime. The new applications will be automatically added to the corresponding team. Therefore, the junior developers that have the permission level **Change and Deploy Applications** for the team can use Service Studio to create modules in the new application.
