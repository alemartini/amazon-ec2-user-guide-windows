# Amazon Machine Images \(AMI\)<a name="AMIs"></a>

An Amazon Machine Image \(AMI\) provides the information required to launch an instance, which is a virtual server in the cloud\. You must specify a source AMI when you launch an instance\. You can launch multiple instances from a single AMI when you need multiple instances with the same configuration\. You can use different AMIs to launch instances when you need instances with different configurations\.

An AMI includes the following:

+ A template for the root volume for the instance \(for example, an operating system, an application server, and applications\)

+ Launch permissions that control which AWS accounts can use the AMI to launch instances

+ A block device mapping that specifies the volumes to attach to the instance when it's launched

## Creating Your Own AMI<a name="creating-an-ami"></a>

You can launch an instance from an existing AMI, customize the instance, and then save this updated configuration as a custom AMI\. Instances launched from this new custom AMI include the customizations that you made when you created the AMI\.

For more information, see [Creating a Custom Windows AMI](Creating_EBSbacked_WinAMI.md)\.

To help categorize and manage your AMIs, you can assign custom *tags* to them\. For more information, see [Tagging Your Amazon EC2 Resources](Using_Tags.md)\.

## Buying, Sharing, and Selling AMIs<a name="buy-share-sell"></a>

After you create an AMI, you can keep it private so that only you can use it, or you can share it with a specified list of AWS accounts\. You can also make your custom AMI public so that the community can use it\. Building a safe, secure, usable AMI for public consumption is a fairly straightforward process, if you follow a few simple guidelines\. For information about how to create and use shared AMIs, see [Shared AMIs](sharing-amis.md)\.

You can purchase AMIs from a third party, including AMIs that come with service contracts from organizations such as Red Hat\. You can also create an AMI and sell it to other Amazon EC2 users\. For more information about buying or selling AMIs, see [Paid AMIs](paid-amis.md)\.

## Deregistering Your AMI<a name="deregistering"></a>

You can deregister an AMI when you have finished with it\. After you deregister an AMI, it can't be used to launch new instances\. Existing instances launched from the AMI are not affected\. For more information, see [Deregistering Your Windows AMI](deregister-ami.md)\.

## AWS Windows AMIs<a name="aws-windows-ami"></a>

AWS provides a set of publicly available AMIs that contain software configurations specific to the Windows platform\. Using these AMIs, you can quickly start building and deploying your applications using Amazon EC2\. First choose the AMI that meets your specific requirements, and then launch an instance using that AMI\. You retrieve the password for the administrator account and then log in to the instance using Remote Desktop Connection, just as you would with any other Windows server\.

Some Windows AMIs include an edition of Microsoft SQL Server \(SQL Enterprise Edition, SQL Server Standard, SQL Server Express, or SQL Server Web\)\. Launching an instance from a Windows AMI with Microsoft SQL Server enables you to run the instance as a database server\. Alternatively, you can launch an instance from any Windows AMI and then install the database software that you need on the instance\.

Microsoft no longer supports Windows Server 2003 \(see [Microsoft Windows Server 2003 End\-of\-Support](https://aws.amazon.com/windows/products/ec2/server2003/)\)\. We recommend that you launch new EC2 instances using a supported version of Windows Server\. If you have existing EC2 instances that are running an unsupported version of Windows Server, we recommend that you upgrade those instances to a supported version of Windows Server\. For more information, see [Upgrading an Amazon EC2 Windows Instance to a Newer Version of Windows Server](serverupgrade.md)\.

### Selecting an Initial Windows AMI<a name="select-windows-ami"></a>

To view the Windows AMIs provided by AWS, you can use the Amazon EC2 console or [AWS Marketplace](https://aws.amazon.com/marketplace/)\. For more information, see [Finding a Windows AMI](finding-an-ami.md)\.

You can also create an AMI from your own Windows computer\. For more information, see the following services:

+ [AWS Server Migration Service](http://docs.aws.amazon.com/server-migration-service/latest/userguide/)

+ [VM Import/Export](http://docs.aws.amazon.com/vm-import/latest/userguide/)

### Keeping Your AMIs Up\-to\-Date<a name="WinAMI_Updating"></a>

AWS provides updated, fully\-patched Windows AMIs within five business days of Microsoft's patch Tuesday \(the second Tuesday of each month\)\. For more information, see [Details About AWS Windows AMI Versions](windows-ami-version-history.md#windows-ami-versions)\.

The AWS Windows AMIs contain the latest security updates available at the time they were created\. For more information, see [Updating Your Windows Instance](windows-ami-version-history.md#update-windows-instance)\.