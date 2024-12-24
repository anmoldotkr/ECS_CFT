## Required IAM Permissions for ECS Tasks and Containers

To successfully run ECS tasks or containers, the following IAM permissions are required for your AWS SSO user or any non-root user. Ensure that your IAM policy includes these permissions:

### IAM Permissions
- **`iam:ListRoles`**: Allows listing of IAM roles.
- **`iam:GetRole`**: Grants permission to retrieve information about a specific IAM role.
- **`iam:ListPolicies`**: Enables listing of IAM policies.
- **`iam:ListRolePolicies`**: Allows listing of inline policies associated with a specific IAM role.
- **`iam:ListAttachedRolePolicies`**: Grants permission to list managed policies attached to a role.
- **`iam:GetPolicyVersion`**: Allows retrieval of a specific version of a managed policy.
- **`iam:PassRole`**: Enables passing a role to an AWS service.

### Amazon ECR Public Permissions
- **`ecr-public:DescribeRepositories`**: Allows describing public ECR repositories.
- **`ecr-public:CreateRepository`**: Grants permission to create a new public ECR repository.

### Amazon CloudWatch Logs Permissions
- **`logs:DescribeLogGroups`**: Allows describing log groups in CloudWatch Logs.

### Access Analyzer Permissions
- **`access-analyzer:ListPolicyGenerations`**: Enables listing of policy generation requests.

### Note
Make sure to review and adjust your IAM policies according to your organization's security best practices. It is recommended to grant the least privilege necessary for users to perform their tasks.

For more information on IAM policies and permissions, refer to the [AWS IAM Documentation](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html).
