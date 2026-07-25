---
api_key_in: []
api_specs:
- filename: amazon-connect-agent-statuses-api-openapi.yml
  format: yaml
  label: Amazon Connect Agent Statuses API
  slug: amazon-connect-agent-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-agent-statuses-api-openapi.yml
- filename: amazon-connect-authentication-api-openapi.yml
  format: yaml
  label: Amazon Connect Authentication API
  slug: amazon-connect-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-authentication-api-openapi.yml
- filename: amazon-connect-contact-flows-api-openapi.yml
  format: yaml
  label: Amazon Connect Contact Flows API
  slug: amazon-connect-contact-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-contact-flows-api-openapi.yml
- filename: amazon-connect-contacts-api-openapi.yml
  format: yaml
  label: Amazon Connect Contacts API
  slug: amazon-connect-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-contacts-api-openapi.yml
- filename: amazon-connect-hours-of-operations-api-openapi.yml
  format: yaml
  label: Amazon Connect Hours of Operations API
  slug: amazon-connect-hours-of-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-hours-of-operations-api-openapi.yml
- filename: amazon-connect-instances-api-openapi.yml
  format: yaml
  label: Amazon Connect Instances API
  slug: amazon-connect-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-instances-api-openapi.yml
- filename: amazon-connect-metrics-api-openapi.yml
  format: yaml
  label: Amazon Connect Metrics API
  slug: amazon-connect-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-metrics-api-openapi.yml
- filename: amazon-connect-queues-api-openapi.yml
  format: yaml
  label: Amazon Connect Queues API
  slug: amazon-connect-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-queues-api-openapi.yml
- filename: amazon-connect-routing-profiles-api-openapi.yml
  format: yaml
  label: Amazon Connect Routing Profiles API
  slug: amazon-connect-routing-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-routing-profiles-api-openapi.yml
- filename: amazon-connect-security-profiles-api-openapi.yml
  format: yaml
  label: Amazon Connect Security Profiles API
  slug: amazon-connect-security-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-security-profiles-api-openapi.yml
- filename: amazon-connect-tags-api-openapi.yml
  format: yaml
  label: Amazon Connect Tags API
  slug: amazon-connect-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-tags-api-openapi.yml
- filename: amazon-connect-users-api-openapi.yml
  format: yaml
  label: Amazon Connect Users API
  slug: amazon-connect-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Connect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Connect secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Connect
provider_slug: amazon-connect
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Requests must be signed using IAM credentials with appropriate Amazon Connect permissions.
  name: aws_signature
  scheme: bearer
  sources:
  - openapi/amazon-connect-openapi.yml
  type: http
slug: amazon-connect-authentication
source_filename: amazon-connect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-connect-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: aws_signature\n  type: http\n  scheme: bearer\n  description: AWS Signature Version 4 authentication. Requests must be signed using IAM credentials\n    with appropriate Amazon Connect permissions.\n  sources:\n  - openapi/amazon-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/authentication/amazon-connect-authentication.yml
summary_line: http · 1 scheme
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
---
