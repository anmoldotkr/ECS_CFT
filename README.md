To run ECS tasks or containers these IAM permission are requied if your SSO USER or if your not root user:

iam:ListRoles
ecr-public:DescribeRepositories
iam:GetRole.
iam:ListPolicies
access-analyzer:ListPolicyGenerations
iam:ListRolePolicies
iam:ListAttachedRolePolicies
iam:GetPolicyVersion
ecr-public:CreateRepository
ecr-public:DescribeRepositories
iam:PassRole
ecr-public:CreateRepository
logs:DescribeLogGroups
