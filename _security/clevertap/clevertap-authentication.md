---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Clevertap Authentication
name_suffix: Authentication
oauth_flows: []
overview: CleverTap secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CleverTap
provider_slug: clevertap
scheme_count: 2
schemes:
- description: CleverTap account identifier
  in: header
  name: AccountId
  parameter: X-CleverTap-Account-Id
  sources:
  - openapi/clevertap-openapi.yml
  type: apiKey
- description: CleverTap account or user passcode
  in: header
  name: Passcode
  parameter: X-CleverTap-Passcode
  sources:
  - openapi/clevertap-openapi.yml
  type: apiKey
slug: clevertap-authentication
source_filename: clevertap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clevertap-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccountId\n  type: apiKey\n  in: header\n  parameter: X-CleverTap-Account-Id\n  description: CleverTap account identifier\n  sources:\n  - openapi/clevertap-openapi.yml\n- name: Passcode\n  type: apiKey\n  in: header\n  parameter: X-CleverTap-Passcode\n  description: CleverTap account or user passcode\n  sources:\n  - openapi/clevertap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/authentication/clevertap-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Audiences
- Customer Engagement
- Customer Retention
- Marketing Automation
- Mobile Engagement
- Push Notifications
- User Behavior
---
