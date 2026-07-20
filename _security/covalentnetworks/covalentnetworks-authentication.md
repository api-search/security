---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Covalentnetworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Covalent secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Covalent
provider_slug: covalentnetworks
scheme_count: 1
schemes:
- mfa: true
  name: AWSCognito
  provider: AWS Cognito
  sources:
  - https://covalentnetworks.com/api-services
  type: oauth2
slug: covalentnetworks-authentication
source_filename: covalentnetworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://covalentnetworks.com/api-services\ndocs: https://covalentnetworks.com/api-services\nsummary:\n  types: [oauth2, openIdConnect]\n  provider: AWS Cognito\n  mfa: true\n  notes: >-\n    Covalent's API is authenticated via AWS Cognito, providing user sign-up,\n    sign-in and access control with multi-factor authentication support and\n    encryption in transit and at rest. No public developer portal exposes the\n    token or authorization endpoints; access is provisioned per tenant. No\n    OpenAPI is published, so this profile is documentation-sourced rather than\n    derived from a spec.\nschemes:\n- name: AWSCognito\n  type: oauth2\n  provider: AWS Cognito\n  mfa: true\n  sources: [https://covalentnetworks.com/api-services]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covalentnetworks/refs/heads/main/authentication/covalentnetworks-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Workforce Operations
- Manufacturing
- Aerospace and Defense
- Skills Management
- Training
- GraphQL
- Enterprise Integration
---
