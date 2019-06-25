# Deploying a NodeJS app to EBS via AWSCLI

In the following example we are going to deploy a simple NodeJS Hello World application to Elastic Beanstalk with command line tools.

### 1. Install the Elastic Beanstalk command line tool

##### Follow these instructions to set up the EBS CLI on your computer: 

* clone the aws-elastic-beanstalk-cli-setup repository from Github:

```
$ git clone https://github.com/aws/aws-elastic-beanstalk-cli-setup.git
```

* run the installer:

```
$ ./aws-elastic-beanstalk-cli-setup/scripts/bundled_installer
```

* follow the instructions in your command line to add the EBS CLI to your PATH!

### 2. Deploy your application with the Elastic Beanstalk command line tool

* configure Elastic Beanstalk in your application's root directory with this command:

```
eb init
```

* when prompted, choose **US-EAST-1 (NORTH VIRGINIA)** as region
* when asked if you want to use **CODE COMMIT**, choose no
* when asked if you want to set up **SSH** for your instances, answer yes
* when prompted, **provide your credentials**

* to create a new environment for your application, use the following command:

```
eb create
```

Follow the prompts.

* and finally, deploy your application:

```
eb deploy
```
