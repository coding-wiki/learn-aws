# Deploying Node.js app to Beanstalk

## Creating Application
1. Open the [Elastic Beanstalk console](https://console.aws.amazon.com/elasticbeanstalk).
2. Choose create a [new application](https://console.aws.amazon.com/elasticbeanstalk/home#/newApplication).
3. Under the **Actions** menu (*top right*), press `Create New Environment`.
4. Choose `Web server environment` out of the two options.
5. 


## SSH Into Application
1. Setup key pair
2. `ssh -i ./path-to-key.pem ec2-user@ec2-some-address.us-west-2.compute.amazonaws.com`
