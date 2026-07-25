---
api_key_in: []
api_specs:
- filename: cloudguard-cloudaccounts-api-openapi.yml
  format: yaml
  label: CloudGuard CloudAccounts API
  slug: cloudguard-cloudaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudguard/refs/heads/main/openapi/cloudguard-cloudaccounts-api-openapi.yml
- filename: cloudguard-compliance-api-openapi.yml
  format: yaml
  label: CloudGuard Compliance API
  slug: cloudguard-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudguard/refs/heads/main/openapi/cloudguard-compliance-api-openapi.yml
- filename: cloudguard-findings-api-openapi.yml
  format: yaml
  label: CloudGuard Findings API
  slug: cloudguard-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudguard/refs/heads/main/openapi/cloudguard-findings-api-openapi.yml
- filename: cloudguard-notifications-api-openapi.yml
  format: yaml
  label: CloudGuard Notifications API
  slug: cloudguard-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudguard/refs/heads/main/openapi/cloudguard-notifications-api-openapi.yml
- filename: cloudguard-policies-api-openapi.yml
  format: yaml
  label: CloudGuard Policies API
  slug: cloudguard-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudguard/refs/heads/main/openapi/cloudguard-policies-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudguard Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudGuard secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudGuard
provider_slug: cloudguard
scheme_count: 1
schemes:
- description: 'CloudGuard authentication uses HTTP Basic with the CloudGuard API

    key id as the username and the API key secret as the password.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cloudguard-openapi.yml
  type: http
slug: cloudguard-authentication
source_filename: cloudguard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudguard-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    CloudGuard authentication uses HTTP Basic with the CloudGuard API\n    key id as the username and the API key secret as the password.\n  sources:\n  - openapi/cloudguard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudguard/refs/heads/main/authentication/cloudguard-authentication.yml
summary_line: http · 1 scheme
tags:
- Check Point
- CNAPP
- Cloud Security
- Compliance
- CSPM
- CWPP
- Posture Management
---
