---
api_key_in:
- header
api_specs:
- filename: checkpoint-access-rules-api-openapi.yml
  format: yaml
  label: Check Point Access Rules API
  slug: checkpoint-access-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-access-rules-api-openapi.yml
- filename: checkpoint-cloud-accounts-api-openapi.yml
  format: yaml
  label: Check Point Cloud Accounts API
  slug: checkpoint-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-cloud-accounts-api-openapi.yml
- filename: checkpoint-compliance-api-openapi.yml
  format: yaml
  label: Check Point Compliance API
  slug: checkpoint-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-compliance-api-openapi.yml
- filename: checkpoint-events-api-openapi.yml
  format: yaml
  label: Check Point Events API
  slug: checkpoint-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-events-api-openapi.yml
- filename: checkpoint-findings-api-openapi.yml
  format: yaml
  label: Check Point Findings API
  slug: checkpoint-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-findings-api-openapi.yml
- filename: checkpoint-hosts-api-openapi.yml
  format: yaml
  label: Check Point Hosts API
  slug: checkpoint-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-hosts-api-openapi.yml
- filename: checkpoint-identity-api-openapi.yml
  format: yaml
  label: Check Point Identity API
  slug: checkpoint-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-identity-api-openapi.yml
- filename: checkpoint-interfaces-api-openapi.yml
  format: yaml
  label: Check Point Interfaces API
  slug: checkpoint-interfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-interfaces-api-openapi.yml
- filename: checkpoint-login-api-openapi.yml
  format: yaml
  label: Check Point Login API
  slug: checkpoint-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-login-api-openapi.yml
- filename: checkpoint-nat-rules-api-openapi.yml
  format: yaml
  label: Check Point NAT Rules API
  slug: checkpoint-nat-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-nat-rules-api-openapi.yml
- filename: checkpoint-networks-api-openapi.yml
  format: yaml
  label: Check Point Networks API
  slug: checkpoint-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-networks-api-openapi.yml
- filename: checkpoint-quarantine-api-openapi.yml
  format: yaml
  label: Check Point Quarantine API
  slug: checkpoint-quarantine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-quarantine-api-openapi.yml
- filename: checkpoint-routes-api-openapi.yml
  format: yaml
  label: Check Point Routes API
  slug: checkpoint-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-routes-api-openapi.yml
- filename: checkpoint-rulesets-api-openapi.yml
  format: yaml
  label: Check Point Rulesets API
  slug: checkpoint-rulesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-rulesets-api-openapi.yml
- filename: checkpoint-services-api-openapi.yml
  format: yaml
  label: Check Point Services API
  slug: checkpoint-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-services-api-openapi.yml
- filename: checkpoint-sessions-api-openapi.yml
  format: yaml
  label: Check Point Sessions API
  slug: checkpoint-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-sessions-api-openapi.yml
- filename: checkpoint-system-api-openapi.yml
  format: yaml
  label: Check Point System API
  slug: checkpoint-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-system-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Checkpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Check Point secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Check Point
provider_slug: checkpoint
scheme_count: 4
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/checkpoint-cloudguard-api-openapi.yml
  type: http
- in: header
  name: sidToken
  parameter: X-chkp-sid
  sources:
  - openapi/checkpoint-gaia-api-openapi.yml
  - openapi/checkpoint-management-api-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/checkpoint-harmony-email-api-openapi.yml
  type: http
- in: header
  name: sharedSecret
  parameter: X-chkp-shared-secret
  sources:
  - openapi/checkpoint-identity-awareness-api-openapi.yml
  type: apiKey
slug: checkpoint-authentication
source_filename: checkpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkpoint-cloudguard-api-openapi.yml, openapi/checkpoint-gaia-api-openapi.yml,\n  openapi/checkpoint-harmony-email-api-openapi.yml, openapi/checkpoint-identity-awareness-api-openapi.yml,\n  openapi/checkpoint-management-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/checkpoint-cloudguard-api-openapi.yml\n- name: sidToken\n  type: apiKey\n  in: header\n  parameter: X-chkp-sid\n  sources:\n  - openapi/checkpoint-gaia-api-openapi.yml\n  - openapi/checkpoint-management-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/checkpoint-harmony-email-api-openapi.yml\n- name: sharedSecret\n  type: apiKey\n  in: header\n  parameter: X-chkp-shared-secret\n  sources:\n  - openapi/checkpoint-identity-awareness-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/authentication/checkpoint-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Cloud Security
- Cybersecurity
- Endpoint Security
- Firewall
- Identity Awareness
- Mobile Security
- Network Security
- Security
- Threat Prevention
- WAF
---
