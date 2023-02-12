# AWS-Cloudformation
DEPLOY CLOUDFORMATION USING AWS CODEPIPELINE \
1- Create codepipeline with existing service role \
2- Create service role (codepipeline is not in the service list, choose ec2 and create role and then edit its trust relationship to codepipeline) \
3- Create inline policy with custom_codepipeline_policy.json \
4- Also add github connection rules to inline policy \
  { \
            "Effect": "Allow", \
            "Action": "codestar-connections:UseConnection", \
            "Resource": "arn:aws:codestar-connections:us-east-1:086796595852:connection/c8b5b6ed-30b0-4d6a-80b7-c1591ec00435" \
        }, \
