---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Commerce Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Salesforce Commerce Cloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Salesforce Commerce Cloud
provider_slug: salesforce-commerce-cloud
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token from SLAS (Shopper APIs) or Salesforce Account

    Manager (Data and Admin APIs), sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-commerce-cloud-openapi.yml
  type: http
slug: salesforce-commerce-cloud-authentication
source_filename: salesforce-commerce-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-commerce-cloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    OAuth 2.0 access token from SLAS (Shopper APIs) or Salesforce Account\n    Manager (Data and Admin APIs), sent as `Authorization: Bearer <token>`.\n  sources:\n  - openapi/salesforce-commerce-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-commerce-cloud/refs/heads/main/authentication/salesforce-commerce-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- E-Commerce
- Headless Commerce
- Salesforce
- B2C Commerce
- B2B Commerce
- Demandware
---
