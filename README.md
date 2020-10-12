# aws-ec2

If you lose the private key for an EBS-backed instance, you can regain access to your instance. You must stop the instance, detach its root volume and attach it to another instance as a data volume, modify the authorized_keys file with a new public key, move the volume back to the original instance, and restart the instance. 

* This procedure is not supported for instances with instance-store backed root volumes. 

To determine the root device type of your instance, open the Amazon EC2 console, choose Instances, select the instance, and check the value of Root device type in the details pane. The value is either ebs or instance store. If the root device is an instance store volume, you cannot use this procedure to regain access to your instance; you must have the private key to connect to the instance. 
