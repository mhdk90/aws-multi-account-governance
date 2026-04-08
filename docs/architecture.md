\# Architecture



```mermaid

flowchart TD

&#x20;   A\[Management Account] --> B\[AWS Organizations]

&#x20;   B --> C\[Root / OU / Member Accounts]

&#x20;   A --> D\[CloudFormation]

&#x20;   D --> E\[Service Control Policy]

&#x20;   A --> F\[CloudTrail - planned]

&#x20;   A --> G\[IAM Identity Center - planned]

