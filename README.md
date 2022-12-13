# Awesome-AWS

## Requirements

## Terminal

### AWS CLI
https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html
```bash
curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
sudo installer -pkg AWSCLIV2.pkg -target /
aws configure
```

### Rain
https://github.com/aws-cloudformation/rain
```bash
brew install rain
```

### Alias
```bash
# aws
AWSFOLDER="$HOME/AWS"
AWSPLAYGROUND="$AWSFOLDER/DEL"
AWSPLAYNAME="del"
AWSPLAYFILE="$AWSPLAYGROUND/$AWSPLAYNAME.yaml"
alias jj='cd $AWSPLAYGROUND'
alias rdp='rain deploy -y $AWSPLAYFILE'
alias rdpc='rain deploy $AWSPLAYFILE'
alias rrm='rain rm -y $AWSPLAYNAME'
alias rf='rain fmt --write $AWSPLAYFILE; rain fmt $AWSPLAYFILE;'
```

## VSCode

### CloudFormation Linter
```bash
pip install cfn-lint
pip install pydot
```
https://github.com/aws-cloudformation/cfn-lint-visual-studio-code

## Cloudformation

- use YAML format
- use AWS::Serverless
  - use AWS::Serverless::Function
  - use AWS::Serverless::Api
  - use AWS::Serverless::Connector
- use Outputs to print info in terminal instead of check in website
