## AWS

[What is AWS?](#what-is-aws)

[Explain the key components of AWS?](#explain-the-key-components-of-aws)

[What is buckets in AWS?](#what-is-buckets-in-aws)

[What is AWS Cloudfront?](#what-is-aws-cloudfront)

[What do you mean by AMI? What does it include?](#what-do-you-mean-by-ami-what-does-it-include)

[How can I download a file from EC2?](#how-can-i-download-a-file-from-ec2)

[Is it possible to clone a EC2 instance data?](#is-it-possible-to-clone-a-ec2-instance-data)

[What is AWS Data Pipeline?](#what-is-aws-data-pipeline)

[Explain the features of Amazon EC2 services](#explain-the-features-of-amazon-ec2-services)

[What is the connection between AMI and Instance?](#what-is-the-connection-between-ami-and-instance)

[Are S3 buckets region specific?](#are-s3-buckets-region-specific)

[What is AWS Direct Connect?](#what-is-aws-direct-connect)

[What is AWS EBS?](#what-is-aws-ebs)

[What is AWS Lambda?](#what-is-aws-lambda)

[What is AWS DynamoDB?](#what-is-aws-dynamodb)

[What is AWS EMR?](#what-is-aws-emr)

[Is data stored in S3 is always encrypted?](#is-data-stored-in-s3-is-always-encrypted)

[Can we attach single EBS to multiple EC2s same time?](#can-we-attach-single-ebs-to-multiple-ec2s-same-time)

[What is AWS API gateway?](#what-is-aws-api-gateway)

[What is AWS Direct Connect?](#what-is-aws-direct-connect)

[What are the security best practices for Amazon EC2 instances?](#what-are-the-security-best-practices-for-amazon-ec2-instances)

[Can I automatically start and terminate my Amazon instance using Amazon API? ](#can-i-automatically-start-and-terminate-my-amazon-instance-using-amazon-api-)

[Can we still continue working on EBS while creating snapshot of it?](#can-we-still-continue-working-on-ebs-while-creating-snapshot-of-it)

[What is AWS Auto Scaling?](#what-is-aws-auto-scaling)

[What is AWS Auto Scaling group?](#what-is-aws-auto-scaling-group)

[What is the maximum size of a single S3 object?](#what-is-the-maximum-size-of-a-single-s3-object)

[What is AWS bucket policy?](#what-is-aws-bucket-policy)

[Does AWS has the option for vertical "auto" scaling of EC2 instance?](#does-aws-has-the-option-for-vertical-auto-scaling-of-ec2-instance)

[What is AWS WAF? What are the potential benefits of using WAF?](#what-is-aws-waf-what-are-the-potential-benefits-of-using-waf)

[How to get the instance id from within an EC2 instance?](#how-to-get-the-instance-id-from-within-an-ec2-instance)

[What is AWS Cloudwatch?](#what-is-aws-cloudwatch)

[What is the difference between Amazon EC2 and AWS Elastic Beanstalk?](#what-is-the-difference-between-amazon-ec2-and-aws-elastic-beanstalk)

[How many storage options are there for EC2 Instance?](#how-many-storage-options-are-there-for-ec2-instance)

[What is AWS Route 53?](#what-is-aws-route-53)

[How would you implement vertical auto scaling of EC2 instance?](#how-would-you-implement-vertical-auto-scaling-of-ec2-instance)

[What is Amazon Kinesis?](#what-is-amazon-kinesis)

[How to find a region from within an EC2 instance?](#how-to-find-a-region-from-within-an-ec2-instance)

[Where are EC2 snapshots stored?](#where-are-ec2-snapshots-stored)

[When should one use the following: Amazon EC2, Google App Engine, Microsoft Azure and Salesforce.com?](#when-should-one-use-the-following-amazon-ec2-google-app-engine-microsoft-azure-and-salesforcecom)

[When to use Amazon CloudFront and when S3?](#when-to-use-amazon-cloudfront-and-when-s3)

[Our EC2 micro instance occasionally runs out of memory. Other than using a larger instance size, what else can be done?](#our-ec2-micro-instance-occasionally-runs-out-of-memory-other-than-using-a-larger-instance-size-what-else-can-be-done)

[What is difference between Lightsail and EC2?](#what-is-difference-between-lightsail-and-ec2)

[What is the underlying hypervisor for EC2?](#what-is-the-underlying-hypervisor-for-ec2)

[How to safely upgrade an Amazon EC2 instance from t1.micro to large?](#how-to-safely-upgrade-an-amazon-ec2-instance-from-t1micro-to-large)



### What is AWS?

**AWS** stands for Amazon Web Services and is a platform that provides database storage, secure cloud services, offering to compute power, content delivery, and many other services to develop business levels.

###### Source

* https://www.onlineinterviewquestions.com/aws-interview-questions/#.W4YpLJMzYsk

[[↑] Back to top](#AWS)
### Explain the key components of AWS?

* **Simple Storage Service (S3)**: S3 is most widely used AWS storage web service.
* **Simple E-mail Service (SES)**: SES is a hosted transactional email service and allows one to fluently send deliverable emails using a RESTFUL API call or through a regular SMTP.
* **Identity and Access Management (IAM)**: IAM provides improved identity and security management for AWS account.
* **Elastic Compute Cloud (EC2)**: EC2 is an AWS ecosystem central piece. It is responsible for providing on-demand and flexible computing resources with a “pay as you go” pricing model.
* **Elastic Block Store (EBS)**: EBS offers continuous storage solution that can be seen in instances as a regular hard drive.
* **CloudWatch**: CloudWatch allows the controller to outlook and gather key metrics and also set a series of alarms to be notified if there is any trouble.

###### Source

* https://www.whizlabs.com/blog/aws-developer-interview-questions/

[[↑] Back to top](#AWS)
### What is buckets in AWS?

An Amazon S3 bucket is a public cloud storage resource available in Amazon Web Services' (AWS) Simple Storage Service (S3), an object storage offering. Amazon S3 buckets, which are similar to file folders, store objects, which consist of data and its descriptive metadata.

By default, you can create up to 100 buckets in each of your AWS accounts. If you need more buckets, you can increase your bucket limit by submitting a service limit increase.

###### Source

* https://www.whizlabs.com/blog/aws-developer-interview-questions/

[[↑] Back to top](#AWS)
### What is AWS Cloudfront?

Amazon **CloudFront** is a content delivery network (CDN) offered by Amazon Web Services. Content delivery networks provide a globally-distributed network of proxy servers which cache content, such as web videos or other bulky media, more locally to consumers, thus improving access speed for downloading the content.

###### Source

* https://en.wikipedia.org/wiki/Amazon_CloudFront

[[↑] Back to top](#AWS)
### What do you mean by AMI? What does it include?

**AMI** stands for the term **Amazon Machine Image**.  It’s an AWS template which provides the information (an application server, and operating system, and applications) required to perform the launch of an instance. This AMI is the copy of the AMI that is running in the cloud as a virtual server.  You can launch instances from as many different AMIs as you need. AMI consists of the followings:

* A root volume template for an existing instance
* Launch permissions to determine which AWS accounts will get the AMI in order to launch the instances
* Mapping for block device to calculate the total volume that will be attached to the instance at the time of launch

###### Source

* https://www.whizlabs.com/blog/aws-developer-interview-questions/

[[↑] Back to top](#AWS)
### How can I download a file from EC2?

Use scp:

```sh
scp -i ec2key.pem username@ec2ip:/path/to/file .
```

###### Source

* https://stackoverflow.com/questions/9441008/how-can-i-download-a-file-from-ec2

[[↑] Back to top](#AWS)
### Is it possible to clone a EC2 instance data?

You can make an AMI of an existing instance, and then launch other instances using that AMI.

###### Source

* 

[[↑] Back to top](#AWS)
### What is AWS Data Pipeline?

**AWS Data Pipeline** is a web service that you can use to automate the movement and transformation of data. With AWS Data Pipeline, you can define data-driven workflows, so that tasks can be dependent on the successful completion of previous tasks.

###### Source

* https://docs.aws.amazon.com/datapipeline/latest/.../what-is-datapipeline.html

[[↑] Back to top](#AWS)
### Explain the features of Amazon EC2 services

Amazon EC2 services have following features:

* Virtual Computing Environments
* Proffers Persistent storage volumes
* Firewall validating you to specify the protocol
* Pre-configured templates
* Static IP address for dynamic Cloud Computing

###### Source

* https://www.whizlabs.com/blog/aws-developer-interview-questions/

[[↑] Back to top](#AWS)
### What is the connection between AMI and Instance?

Many different types of *instances* can be launched from one *AMI*. The type of an instance generally regulates the hardware components of the host computer that is used for the instance. Each type of instance has distinct computing and memory efficacy.

Once an instance is launched, it casts as host and the user interaction with it is same as with any other computer but we have a completely controlled access to our instances. AWS developer interview questions may contain one or more AMI based questions, so prepare yourself for the AMI topic very well.

###### Source

* https://www.whizlabs.com/blog/aws-developer-interview-questions/

[[↑] Back to top](#AWS)
### Are S3 buckets region specific?

Yes, buckets exist in a specific region and you need to specify that region when you create a bucket. Amazon S3 creates bucket in a region you specify. You can choose any AWS region that is geographically close to you to optimize latency, minimize costs, or address regulatory requirements.

###### Source

* https://stackoverflow.com/questions/36754094/are-s3-buckets-region-specific

[[↑] Back to top](#AWS)
### What is AWS Direct Connect?

**AWS Direct Connect** bypasses the public Internet and establishes a secure, dedicated connection from your infrastructure into AWS. With established connectivity via AWS Direct Connect, you can access your Amazon VPC and all AWS services.

###### Source

* https://www.coresite.com/resources/blog/january.../vpn-or-direct-connect-aws-compared

[[↑] Back to top](#AWS)
### What is AWS EBS?

**Amazon Elastic Block Store** (Amazon EBS) provides persistent block storage volumes for use with Amazon EC2 instances in the AWS Cloud. Each Amazon EBS volume is automatically replicated within its Availability Zone to protect you from component failure, offering high availability and durability.

###### Source

* https://aws.amazon.com/ebs/

[[↑] Back to top](#AWS)
### What is AWS Lambda?

**AWS Lambda** is a serverless compute service that runs your code in response to events and automatically manages the underlying compute resources for you. You can use AWS Lambda to extend other AWS services with custom logic, or create your own back-end services that operate at AWS scale, performance, and security.

###### Source

* https://aws.amazon.com/lambda/features/

[[↑] Back to top](#AWS)
### What is AWS DynamoDB?

**Amazon DynamoDB** is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability. With DynamoDB, you can create database tables that can store and retrieve any amount of data, and serve any level of request traffic.

###### Source

* https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html

[[↑] Back to top](#AWS)
### What is AWS EMR?

**Amazon Elastic MapReduce (EMR)** is an Amazon Web Services (AWS) tool for big data processing and analysis. Amazon EMR offers the expandable low-configuration service as an easier alternative to running in-house cluster computing.

Amazon EMR is based on Apache Hadoop, a Java-based programming framework that supports the processing of large data sets in a distributed computing environment. MapReduce is a software framework that allows developers to write programs that process massive amounts of unstructured data in parallel across a distributed cluster of processors or stand-alone computers.

###### Source

* https://searchaws.techtarget.com/definition/Amazon-Elastic-MapReduce-Amazon-EMR

[[↑] Back to top](#AWS)
### Is data stored in S3 is always encrypted?

By default data on S3 is not encrypted, but all you could enable server-side encryption in your object metadata when you upload your data to Amazon S3. As soon as your data reaches S3, it is encrypted and stored.

###### Source

* https://aws.amazon.com/blogs/developer/data-encryption-with-amazon-s3/

[[↑] Back to top](#AWS)
### Can we attach single EBS to multiple EC2s same time?

No. After you create a volume, you can attach it to any EC2 instance in the same Availability Zone. An EBS volume can be attached to **only one EC2 instance at a time**, but multiple volumes can be attached to a single instance.

###### Source

* https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSVolumes.html

[[↑] Back to top](#AWS)
### What is AWS API gateway?

Amazon **API Gateway** is an AWS service that enables developers to create, publish, maintain, monitor, and secure APIs at any scale. You can create APIs that access AWS or other web services, as well as data stored in the AWS Cloud.

###### Source

* https://aws.amazon.com/directconnect/

[[↑] Back to top](#AWS)
### What is AWS Direct Connect?

Using **AWS Direct Connect**, you can establish private connectivity between AWS and your datacenter, office, or colocation environment, which in many cases can reduce your network costs, increase bandwidth throughput, and provide a more consistent network experience than Internet-based connections.

###### Source

* https://aws.amazon.com/directconnect/

[[↑] Back to top](#AWS)
### What are the security best practices for Amazon EC2 instances?

There are a number of best practices for securing Amazon EC2 instances that are applicable whether instances are running on on-premise data centers or on virtual machines. Let’s have a look at some general best practices:

**Least Access**: Make sure that your EC2 instance has controlled access to the instance as well as to the network. Offer access authorities only to the trusted entities.

**Least Privilege**: Follow the necessary principle of least privilege for instances and users to perform the functions. Generate roles with restricted access for the instances.

**Configuration Management**: Consider every EC2 instance a configuration item and use AWS configuration management services to have a baseline for the configuration of the instances as these services include updated anti-virus software, security features etc.

###### Source

* https://www.whizlabs.com/blog/aws-developer-interview-questions/

[[↑] Back to top](#AWS)
### Can I automatically start and terminate my Amazon instance using Amazon API? 

You can achieve it by adding a schedule to an auto scaling group: increase the amount of instances in an auto scaling group to 1 at certain times and decrease it back to 0 afterwards.

###### Source

* https://stackoverflow.com/questions/2413029/auto-shutdown-and-start-amazon-ec2-instance

[[↑] Back to top](#AWS)
### Can we still continue working on EBS while creating snapshot of it?

When a **snapshot** is created from a volume with an AWS Marketplace product code, the product code is propagated to the snapshot. So yes, you can take a snapshot of an attached volume that is in use. However, snapshots only capture data that has been written to your Amazon EBS volume at the time the snapshot command is issued.

###### Source

* https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-creating-snapshot.html

[[↑] Back to top](#AWS)
### What is AWS Auto Scaling?

AWS CodeDeploy supports **Auto Scaling**, an AWS service that can launch Amazon EC2 instances automatically according to conditions you define. These conditions can include limits exceeded in a specified time interval for CPU utilization, disk reads or writes, or inbound or outbound network traffic.

###### Source

* https://docs.aws.amazon.com/codedeploy/latest/.../integrations-aws-auto-scaling.html

[[↑] Back to top](#AWS)
### What is AWS Auto Scaling group?

An **Auto Scaling group** contains a collection of EC2 instances that share similar characteristics and are treated as a logical grouping for the purposes of instance scaling and management. 

For example, if a single application operates across multiple instances, you might want to increase the number of instances in that group to improve the performance of the application, or decrease the number of instances to reduce costs when demand is low. 

You can use the Auto Scaling group to scale the number of instances automatically based on criteria that you specify, or maintain a fixed number of instances even if an instance becomes unhealthy.

###### Source

* https://docs.aws.amazon.com/autoscaling/ec2/userguide/AutoScalingGroup.html

[[↑] Back to top](#AWS)
### What is the maximum size of a single S3 object?

Individual Amazon S3 objects can range in size from a minimum of 0 bytes to a **maximum of 5 terabytes**. The largest object that can be uploaded in a single PUT is 5 gigabytes. For objects larger than 100 megabytes, customers should consider using the Multipart Upload capability.

###### Source

* https://aws.amazon.com/s3/faqs/

[[↑] Back to top](#AWS)
### What is AWS bucket policy?

A *bucket policy* is a resource-based AWS Identity and Access Management (IAM) policy. You add a bucket policy to a bucket to grant other AWS accounts or IAM users access permissions for the bucket and the objects in it. Object permissions apply only to the objects that the bucket owner creates.

###### Source

* https://docs.aws.amazon.com/AmazonS3/latest/user-guide/add-bucket-policy.html

[[↑] Back to top](#AWS)
### Does AWS has the option for vertical "auto" scaling of EC2 instance?

No, this is not native available within EC2 Auto Scaling Groups. AWS does allow you to Vertically scale by changing the instance type from a Lower Instance type to a higher one. But it has it's own disadvantages:

* You need to stop the instance to actually change the instance type
* If your existing instance is of virtualization type PV, you can only choose an instance that is also of the type PV
* If your existing instance is a reserved instance with upfront payment, then you can only scale it to an instance of the same instance family (for example m1 and m3 etc)



###### Source

* https://www.quora.com/Does-Amazon-AWS-has-the-option-for-vertical-auto-scaling-of-EC2-instance

[[↑] Back to top](#AWS)
### What is AWS WAF? What are the potential benefits of using WAF?

**AWS WAF** is a web application firewall that lets you monitor the HTTP and HTTPS applications that are promoted to Amazon CloudFront and gives you regulate path to your content. Based on circumstances that you stipulate, such as the IP addresses that grants originate from or the consequences of query series, CloudFront returns to applications either with the petitioned content or with an HTTP 403 situation code (Forbidden). You can further configure CloudFront to restore a pattern failure page when an application is obstructed.

Advantages of utilizing WAF:

* Further security versus web initiatives relating circumstances that you designate. You can describe situations by managing characteristics of web inquiries such as the IP address that the applications originate from, the rates in headers, chains that rise in the applications, and the presence of hateful SQL code in the call, which is recognized as SQL injection.
* Rules that you can reuse for various network appeals
* Real-time metrics and examined web demands
* Computerized command practicing the AWS WAF API

###### Source

* https://svrtechnologies.com/aws-interview-questions/top-50-aws-interview-questions-and-answers-pdf

[[↑] Back to top](#AWS)
### How to get the instance id from within an EC2 instance?

Run:
```sh
wget -q -O - http://169.254.169.254/latest/meta-data/instance-id
```

Or on Amazon Linux AMIs you can do:
```sh
$ ec2-metadata -i
instance-id: i-1234567890abcdef0
```

###### Source

* https://stackoverflow.com/questions/625644/how-to-get-the-instance-id-from-within-an-ec2-instance

[[↑] Back to top](#AWS)
### What is AWS Cloudwatch?

**Amazon CloudWatch** is a monitoring service for AWS cloud resources and the applications you run on AWS. You can use Amazon CloudWatch to collect and track metrics, collect and monitor log files, set alarms, and automatically react to changes in your AWS resources.

###### Source

* https://www.youtube.com/watch?v=_Tqce6pGb44

[[↑] Back to top](#AWS)
### What is the difference between Amazon EC2 and AWS Elastic Beanstalk?

* **EC2** is Amazon's service that allows you to create a server (AWS calls these instances) in the AWS cloud. You pay by the hour and only what you use. You can do whatever you want with this instance as well as launch n number of instances.

* **Elastic Beanstalk** is one layer of abstraction away from the EC2 layer. Elastic Beanstalk will setup an "environment" for you that can contain a number of EC2 instances, an optional database, as well as a few other AWS components such as a Elastic Load Balancer, Auto-Scaling Group, Security Group. Then Elastic Beanstalk will manage these items for you whenever you want to update your software running in AWS. 

###### Source

* https://stackoverflow.com/questions/25956193/difference-between-amazon-ec2-and-aws-elastic-beanstalk

[[↑] Back to top](#AWS)
### How many storage options are there for EC2 Instance?

There are four storage options for Amazon EC2 Instance:

* Amazon EBS
* Amazon EC2 Instance Store
* Amazon S3
* Adding Storage

###### Source

* https://www.whizlabs.com/blog/aws-developer-interview-questions/

[[↑] Back to top](#AWS)
### What is AWS Route 53?

**Amazon Route 53** (Route 53) is a scalable and highly available Domain Name System (DNS). AWS supposedly named the service Route 53 because all DNS requests are handled through port 53, and the "route" piece resembles the historic "Route 66" of the USA. Presumably because DNS queries are handled on "well-known port" 53.

###### Source

* https://docs.aws.amazon.com/codedeploy/latest/.../integrations-aws-auto-scaling.html

[[↑] Back to top](#AWS)
### How would you implement vertical auto scaling of EC2 instance?

Vertical auto scaling is not native available within EC2 Auto Scaling Groups.

However this is certainly very possible to be accomplished all within AWS. AWS Atuo Scaling Groups use a Launch Configuration. You can change which launch configuration you are using for an auto scaling group. So you can create two launch configurations. Call one "t2.medium" and the other "m3.medium" with the relative instance type associated and then update which launch configuration is used for the auto scaling group. To actually scale up you would then need to force some scale up and down events to get rid of the older t2.medium instances.

My suggestion would be to build this in to a couple of Lambda functions. First function updates the launch configuration and the subsequent function(s) scale up and/or down the group in order to ensure that all running instances are of the desired new size.

###### Source

* https://www.quora.com/Does-Amazon-AWS-has-the-option-for-vertical-auto-scaling-of-EC2-instance

[[↑] Back to top](#AWS)
### What is Amazon Kinesis?

**Amazon Kinesis** is an Amazon Web Service (AWS) for processing big data in real time. Kinesis is capable of processing hundreds of terabytes per hour from high volumes of streaming data from sources such as operating logs, financial transactions and social media feeds.

###### Source

* https://searchaws.techtarget.com/definition/Amazon-Kinesis

[[↑] Back to top](#AWS)
### How to find a region from within an EC2 instance?

Consider:
```sh
EC2_AVAIL_ZONE=`curl -s http://169.254.169.254/latest/meta-data/placement/availability-zone`
EC2_REGION="`echo \"$EC2_AVAIL_ZONE\" | sed 's/[a-z]$//'`"
```

###### Source

* https://stackoverflow.com/questions/4249488/find-region-from-within-an-ec2-instance

[[↑] Back to top](#AWS)
### Where are EC2 snapshots stored?

EBS snapshots are stored in S3 but not in a user-visible bucket. To view your snapshots use the AWS api or they are in the EC2/Snapshots tab of the AWS Console. Something like: 

```sh
https://console.aws.amazon.com/ec2/home?region=us-east-1#s=Snapshots
```

depending on your region.

###### Source

* https://stackoverflow.com/questions/5227791/why-cant-i-see-my-ebs-volume-snapshots-in-s3-from-aws-management-console

[[↑] Back to top](#AWS)
### When should one use the following: Amazon EC2, Google App Engine, Microsoft Azure and Salesforce.com?

* **EC2** is Infrastructure as a Service; you get VM instances, and do with them as you wish. Rackspace Cloud Servers are more or less the same.

* Azure, App Engine, and Salesforce are all Platform as a Service; they offer different levels of integration, though: Azure pretty much lets you run arbitrary background services, while App Engine is oriented around short lived request handler tasks (though it also supports a task queue and scheduled tasks). I'm not terribly familiar with Salesforce's offering, but my understanding is that it's similar to App Engine in some respects, though more specialized for its particular niche.

###### Source

* 

[[↑] Back to top](#AWS)
### When to use Amazon CloudFront and when S3?

**Amazon S3** is designed for large-capacity, low-cost file storage in one specific geographical region. The storage and bandwidth costs are quite low.

**Amazon CloudFront** is a Content Delivery Network (CDN) which proxies and caches web data at edge locations as close to users as possible.

f your user base is *localized*, you won't see too much difference working with S3 or CloudFront (but you have to choose the right location for your S3 bucket: US, EU, APAC). If your user base is spread *globally* and speed is important, CloudFront may be a better option.

###### Source

* https://stackoverflow.com/questions/5898308/how-to-safely-upgrade-an-amazon-ec2-instance-from-t1-micro-to-large

[[↑] Back to top](#AWS)
### Our EC2 micro instance occasionally runs out of memory. Other than using a larger instance size, what else can be done?

A fix for this problem is to add `swap` (i.e. `paging`) space to the instance.

Paging works by creating an area on your hard drive and using it for extra memory, this memory is much slower than normal memory however much more of it is available.

To add this extra space to your instance you type:
```sh
sudo /bin/dd if=/dev/zero of=/var/swap.1 bs=1M count=1024
sudo /sbin/mkswap /var/swap.1
sudo chmod 600 /var/swap.1
sudo /sbin/swapon /var/swap.1
```
If you need more than 1024 then change that to something higher.

To enable it by default after reboot, add this line to `/etc/fstab`:

```sh
 /var/swap.1   swap    swap    defaults        0   0
```

###### Source

* 

[[↑] Back to top](#AWS)
### What is difference between Lightsail and EC2?

**Lightsail VPSs** are bundles of existing AWS products, offered through a significantly simplified interface. The difference is that Lightsail offers you a limited and fixed menu of options but with much greater ease of use. Other than the narrower scope of Lightsail in order to meet the requirements for simplicity and low cost, the underlying technology is the same.

Testing reveals that Lightsail instances in fact are EC2 instances, from the t2 class of burstable instances.

###### Source

* https://stackoverflow.com/questions/40927189/what-is-difference-between-lightsail-and-ec2

[[↑] Back to top](#AWS)
### What is the underlying hypervisor for EC2?

Every AWS AMI uses the Xen hypervisor on bare metal. Xen offers two kinds of virtualization: 
* HVM (Hardware Virtual Machine)
* PV (Paravirtualization). 

Virtual machines (also known as Guests) run on top of a hypervisor.

###### Source

* https://cloudacademy.com/blog/aws-ami-hvm-vs-pv-paravirtual-amazon/

[[↑] Back to top](#AWS)
### How to safely upgrade an Amazon EC2 instance from t1.micro to large?

Follow the procedure:

1. Create a snapshot of current instance image 
2. Launch the new instance as a large instance at that point. 
3. Disassociate the ip with the old instance and then associate it with the new one
4. Once if sure everything is running fine, delete the old instance (because there's no dependency between the two instance). 

This is the right approach if you do not want any downtime (i.e. production server) because this solution only takes a server offline only after the new one is up and running. 

If you are using elastic IP as you should, assign the elastic IP to the new server. The new server will then have the same IP address. 

Please also note that the server state might change if it's under stress (which is very likely considering the need to scale it up), and the new, larger server will be a few minutes/hours older than the actual running server. 


###### Source

* https://stackoverflow.com/questions/5898308/how-to-safely-upgrade-an-amazon-ec2-instance-from-t1-micro-to-large

[[↑] Back to top](#AWS)
