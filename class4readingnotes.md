Gary King
09/01/2022
Class 4 Reading Notes
What is Group Policy (GPO) & What Role Does It Play in Data Security

Group Policies Objet (GPO)is a feature  Windows that does a variety of advanced settings that the network admins can use to control the working environment.of users.
It creates a centralized location for the admin to manage and configure operating systems, applications and user settings.

If GPO is used properly you can increase security of users computers to help fight external attacks as well as any possible internal attacks.
The GPO is actually a group of settings that is created using the Microsoft Management Console (MMC) Group Policy EditorA GPO could be used to show a certain home page when launching a web browser or show a certain list of printers that are specific to your network.
An admin could also install a number of security features like restricting certain internet connections and programs that can be ran.
The order that GPOs are processed affects what settings are applied to a computer and also to a user.

The local computer policy is the first to be processed then followed by the site level domain AD policies and then into the organization units.
You need to have GPOs because Windows straight out of the box has numerous holes in the system that need to be filled and that happens with implementing the GPOs
Like setting up a use you can give them only privileges just to only do their particular job.
We can set user passwords to be updated every 30 days to help reduce the risk of being hacked from an old user password.

When adding new computers to the system you speed the process up by having the GPO set up so that every computer has the basic set up and then you just add what needs to be for each user, or each department.
GPO can also deploy software updates throughout the system without having to each one individually. And that way every computer will be uptodate against the latest security threats .

GPOs is not a user friendly console but if you have a deep understanding of PowerShell this will help working the system.
