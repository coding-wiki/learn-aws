# Deploying Node.js app to Beanstalk

## Creating Application
1. Open the [Elastic Beanstalk console](https://console.aws.amazon.com/elasticbeanstalk).
1. Choose create a [new application](https://console.aws.amazon.com/elasticbeanstalk/home#/newApplication).
1. Under the **Actions** menu (*top right*), press `Create New Environment`.
1. Choose `Web server environment` out of the two options.
1. 

## Setup EB CLI
**Using Homebrew**
```sh
brew install awsebcli
```

**Using pip**
1. Install Elastic Beanstalk CLI with:
```sh
pip install awsebcli --upgrade --user
# Where:
# --upgrade upgrades dependencies
# --user installs the program under your user dir (doesn't touch system libraries)
```
(if using `brew`: use `pip2` or `pip3` depending on your Python (2/3.x) version
1. Add to your `PATH` variable:
```
export PATH=~/Library/Python/2.7/bin:$PATH
# Where 2.7 is your corresponding Python version
```
**Upgrading EB CLI**
1. In your CLI, run:
```sh
pip install awsebcli --upgrade --user
```


## SSH Into Application
1. Setup key pair
1. `ssh -i ./path-to-key.pem ec2-user@ec2-some-address.us-west-2.compute.amazonaws.com`
