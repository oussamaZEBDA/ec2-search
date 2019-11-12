# ec2-search
Read in an AWS credentials file and iterate through each account, saving details on every instance (in every region) to disk. We cant then quickly query this information to provide get on EC2 instances without having to log into AWS or use the AWS CLI.

## Installation

## Usage
### Load
Read throught the users credential file *(~/.aws/credentials)* and save information about every instance found to a pickled Python object.
```
ec2-search load
```

### Search
Search the stored results to find a keyword (based on instance tag values).
```
ec2-search search [searchterm]
```

