# AWS-Cloudformation
DEPLOY CLOUDFORMATION USING AWS CODEPIPELINE \
1- Create codepipeline with existing service role \
2- Create service role (codepipeline is not in the service list, choose ec2 and create role and then edit its trust relationship to codepipeline) \
3- Create inline policy with custom_codepipeline_policy.json \
4- Also allow to use github connection (apply tihs to same policy) \
  { \
            "Effect": "Allow", \
            "Action": "codestar-connections:UseConnection", \
            "Resource": "arn:aws:codestar-name" \
        }, 
