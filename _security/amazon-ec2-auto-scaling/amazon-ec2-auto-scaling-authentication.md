---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-ec2-auto-scaling-auto-scaling-group-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Auto Scaling Group API
  slug: amazon-ec2-auto-scaling-auto-scaling-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-auto-scaling-group-api-openapi.yml
- filename: amazon-ec2-auto-scaling-launch-configuration-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Launch Configuration API
  slug: amazon-ec2-auto-scaling-launch-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-launch-configuration-api-openapi.yml
- filename: amazon-ec2-auto-scaling-lifecycle-hook-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Lifecycle Hook API
  slug: amazon-ec2-auto-scaling-lifecycle-hook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-lifecycle-hook-api-openapi.yml
- filename: amazon-ec2-auto-scaling-load-balancer-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Load Balancer API
  slug: amazon-ec2-auto-scaling-load-balancer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-load-balancer-api-openapi.yml
- filename: amazon-ec2-auto-scaling-load-balancer-target-group-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Load Balancer Target Group API
  slug: amazon-ec2-auto-scaling-load-balancer-target-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-load-balancer-target-group-api-openapi.yml
- filename: amazon-ec2-auto-scaling-notification-configuration-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Notification Configuration API
  slug: amazon-ec2-auto-scaling-notification-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-notification-configuration-api-openapi.yml
- filename: amazon-ec2-auto-scaling-operations-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Operations API
  slug: amazon-ec2-auto-scaling-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-operations-api-openapi.yml
- filename: amazon-ec2-auto-scaling-policy-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Policy API
  slug: amazon-ec2-auto-scaling-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-policy-api-openapi.yml
- filename: amazon-ec2-auto-scaling-scaling-plan-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Scaling Plan API
  slug: amazon-ec2-auto-scaling-scaling-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-scaling-plan-api-openapi.yml
- filename: amazon-ec2-auto-scaling-scheduled-action-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Scheduled Action API
  slug: amazon-ec2-auto-scaling-scheduled-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-scheduled-action-api-openapi.yml
- filename: amazon-ec2-auto-scaling-traffic-source-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Traffic Source API
  slug: amazon-ec2-auto-scaling-traffic-source-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-traffic-source-api-openapi.yml
- filename: amazon-ec2-auto-scaling-warm-pool-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Warm Pool API
  slug: amazon-ec2-auto-scaling-warm-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-warm-pool-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon EC2 Auto Scaling Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EC2 Auto Scaling secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-ec2-auto-scaling-auto-scaling-group-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-launch-configuration-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-lifecycle-hook-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-load-balancer-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-load-balancer-target-group-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-notification-configuration-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-operations-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-policy-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-scaling-plan-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-scheduled-action-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-traffic-source-api-openapi.yml
  - openapi/amazon-ec2-auto-scaling-warm-pool-api-openapi.yml
  type: apiKey
slug: amazon-ec2-auto-scaling-authentication
source_filename: amazon-ec2-auto-scaling-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-ec2-auto-scaling-auto-scaling-group-api-openapi.yml, openapi/amazon-ec2-auto-scaling-launch-configuration-api-openapi.yml,\n  openapi/amazon-ec2-auto-scaling-lifecycle-hook-api-openapi.yml, openapi/amazon-ec2-auto-scaling-load-balancer-api-openapi.yml,\n  openapi/amazon-ec2-auto-scaling-load-balancer-target-group-api-openapi.yml, openapi/amazon-ec2-auto-scaling-notification-configuration-api-openapi.yml,\n  openapi/amazon-ec2-auto-scaling-operations-api-openapi.yml, openapi/amazon-ec2-auto-scaling-policy-api-openapi.yml,\n  openapi/amazon-ec2-auto-scaling-scaling-plan-api-openapi.yml, openapi/amazon-ec2-auto-scaling-scheduled-action-api-openapi.yml,\n  openapi/amazon-ec2-auto-scaling-traffic-source-api-openapi.yml, openapi/amazon-ec2-auto-scaling-warm-pool-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n\
  \  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-ec2-auto-scaling-auto-scaling-group-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-launch-configuration-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-lifecycle-hook-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-load-balancer-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-load-balancer-target-group-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-notification-configuration-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-operations-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-policy-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-scaling-plan-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-scheduled-action-api-openapi.yml\n  - openapi/amazon-ec2-auto-scaling-traffic-source-api-openapi.yml\n\
  \  - openapi/amazon-ec2-auto-scaling-warm-pool-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-ec2-auto-scaling/authentication/amazon-ec2-auto-scaling-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Auto-Scaling
- Compute
- EC2
- High Availability
- Scaling
---
