# Upgrading an Amazon EC2 Windows Instance to a Newer Version of Windows Server<a name="serverupgrade"></a>

There are two methods to upgrade an earlier version of Windows Server running on an instance: in\-place upgrade and migration \(also called side\-by\-side upgrade\)\. An in\-place upgrade upgrades the operating system files while your personal settings and files are intact\. A migration involves capturing settings, configurations, and data and porting these to a newer operating system on a fresh Amazon EC2 instance\.

Microsoft has traditionally recommended migrating to a newer version of Windows Server instead of upgrading\. Migrating can result in fewer upgrade errors or issues, but can take longer than an in\-place upgrade because of the need to provision a new instance, plan for and port applications, and adjust configurations settings on the new instance\. An in\-place upgrade can be faster, but software incompatibilities can produce errors\.


+ [Performing a Server Migration](os-migration.md)
+ [Performing an In\-Place Upgrade](os-inplaceupgrade.md)
+ [Troubleshooting an Upgrade](os-upgrade-trbl.md)