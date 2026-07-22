---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Trax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trax secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trax
provider_slug: trax
scheme_count: 3
schemes:
- description: Trax platform username and password used for direct partner API authentication.
  name: TraxCredentials
  scheme: basic
  sources:
  - docs
  type: http
- description: Single Sign-On using the OAuth 2.0 protocol against a customer-configured authentication server. Documented identity-provider integrations include ADFS, Salesforce (SFDC), Okta, and Ping Federate.
  identity_providers:
  - ADFS
  - Salesforce
  - Okta
  - Ping Federate
  name: SSO
  sources:
  - docs
  type: oauth2
- description: Daily token requested from the Trax license-management system by the Scene Mobile SDK to verify eligibility to use the SDK on a given day (Android and iOS).
  name: SceneSDKDailyToken
  scheme: bearer
  sources:
  - docs
  type: http
slug: trax-authentication
source_filename: trax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.apidoc.traxretail.com/\ndocs: https://www.apidoc.traxretail.com/\nsummary:\n  types:\n  - http\n  - oauth2\n  notes: >-\n    Partner API access authenticates with Trax platform credentials (username and password) or via\n    Single Sign-On over OAuth 2.0. The Scene Mobile SDK additionally requests a per-day license\n    token from the Trax license-management system to authorize SDK use for that calendar day.\nschemes:\n- name: TraxCredentials\n  type: http\n  scheme: basic\n  description: Trax platform username and password used for direct partner API authentication.\n  sources:\n  - docs\n- name: SSO\n  type: oauth2\n  description: >-\n    Single Sign-On using the OAuth 2.0 protocol against a customer-configured authentication server.\n    Documented identity-provider integrations include ADFS, Salesforce (SFDC), Okta, and Ping\n    Federate.\n  identity_providers:\n  - ADFS\n  - Salesforce\n  - Okta\n  - Ping\
  \ Federate\n  sources:\n  - docs\n- name: SceneSDKDailyToken\n  type: http\n  scheme: bearer\n  description: >-\n    Daily token requested from the Trax license-management system by the Scene Mobile SDK to verify\n    eligibility to use the SDK on a given day (Android and iOS).\n  sources:\n  - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trax/refs/heads/main/authentication/trax-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Enterprise
- Retail
- Computer Vision
- Image Recognition
- CPG
- Retail Execution
- Merchandising
- SaaS
---
