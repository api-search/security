---
api_key_in:
- header
api_specs:
- filename: magic-moment-salesforce-integration-openapi.yml
  format: yaml
  label: Magic Moment Playbook Salesforce Integration API
  slug: magic-moment-playbook-salesforce-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-salesforce-integration-openapi.yml
- filename: magic-moment-hubspot-integration-openapi.yml
  format: yaml
  label: Magic Moment Playbook HubSpot Integration API
  slug: magic-moment-playbook-hubspot-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-hubspot-integration-openapi.yml
- filename: magic-moment-office-suite-integration-openapi.yml
  format: yaml
  label: Magic Moment Playbook Office Suite Integration API
  slug: magic-moment-playbook-office-suite-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-office-suite-integration-openapi.yml
- filename: magic-moment-call-integration-openapi.yml
  format: yaml
  label: Magic Moment Playbook Call Integration API
  slug: magic-moment-playbook-call-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-call-integration-openapi.yml
- filename: magic-moment-reporting-openapi.yml
  format: yaml
  label: Magic Moment Playbook Reporting API
  slug: magic-moment-playbook-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-reporting-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Magic Moment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magic Moment secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Magic Moment
provider_slug: magic-moment
scheme_count: 2
schemes:
- in: header
  name: accessToken
  parameter: x-access-token
  sources:
  - openapi/magic-moment-call-integration-openapi.yml
  - openapi/magic-moment-hubspot-integration-openapi.yml
  - openapi/magic-moment-office-suite-integration-openapi.yml
  - openapi/magic-moment-reporting-openapi.yml
  - openapi/magic-moment-salesforce-integration-openapi.yml
  type: apiKey
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/magic-moment-hubspot-integration-openapi.yml
  - openapi/magic-moment-office-suite-integration-openapi.yml
  - openapi/magic-moment-reporting-openapi.yml
  - openapi/magic-moment-salesforce-integration-openapi.yml
  type: apiKey
slug: magic-moment-authentication
source_filename: magic-moment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/magic-moment-call-integration-openapi.yml, openapi/magic-moment-hubspot-integration-openapi.yml,\n  openapi/magic-moment-office-suite-integration-openapi.yml, openapi/magic-moment-reporting-openapi.yml,\n  openapi/magic-moment-salesforce-integration-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: x-access-token\n  sources:\n  - openapi/magic-moment-call-integration-openapi.yml\n  - openapi/magic-moment-hubspot-integration-openapi.yml\n  - openapi/magic-moment-office-suite-integration-openapi.yml\n  - openapi/magic-moment-reporting-openapi.yml\n  - openapi/magic-moment-salesforce-integration-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/magic-moment-hubspot-integration-openapi.yml\n  - openapi/magic-moment-office-suite-integration-openapi.yml\n  - openapi/magic-moment-reporting-openapi.yml\n\
  \  - openapi/magic-moment-salesforce-integration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/authentication/magic-moment-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Enterprise
- Sales
- Artificial Intelligence
- CRM
- Sales Automation
- Software-as-a-Service
- Japan
- Salesforce
- HubSpot
- Sales Enablement
---
