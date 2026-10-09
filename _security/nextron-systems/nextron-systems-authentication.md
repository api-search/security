---
anonymous_access: true
api_key_in: []
api_specs:
- filename: nextron-systems-info-api-openapi.yml
  format: yaml
  label: Nextron Systems Info API
  slug: nextron-systems-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextron-systems/refs/heads/main/openapi/nextron-systems-info-api-openapi.yml
- filename: nextron-systems-results-api-openapi.yml
  format: yaml
  label: Nextron Systems Results API
  slug: nextron-systems-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextron-systems/refs/heads/main/openapi/nextron-systems-results-api-openapi.yml
- filename: nextron-systems-scan-api-openapi.yml
  format: yaml
  label: Nextron Systems Scan API
  slug: nextron-systems-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextron-systems/refs/heads/main/openapi/nextron-systems-scan-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Nextron Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nextron Systems declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Nextron Systems
provider_slug: nextron-systems
scheme_count: 3
schemes:
- api: nextron-systems:thor-thunderstorm-api
  description: No authentication declared in the contract; self-hosted service on the customer's network.
  name: none
  sources:
  - openapi/nextron-systems-thunderstorm-openapi.yml
  - https://thor-manual.nextron-systems.com/en/latest/usage/deployment.html
  type: none
- api: nextron-systems:analysis-cockpit-api
  description: To test the API in the web interface, copy the API key from your user settings into the key field. Header/parameter name is not published outside the appliance.
  name: Analysis Cockpit API key
  sources:
  - https://analysis-cockpit-manual.nextron-systems.com/en/latest/administration/api.html
  type: apiKey
- api: nextron-systems:asgard-management-center-api
  description: 'Licensing endpoint example: curl -XPOST "https://my-asgard.internal:8443/api/v0/licensing/issue?token=..." (download token configured under Downloads > Download Token Configuration).'
  in: query
  name: ASGARD download token
  parameter: token
  sources:
  - https://thor-manual.nextron-systems.com/en/latest/usage/deployment.html
  type: apiKey
slug: nextron-systems-authentication
source_filename: nextron-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://analysis-cockpit-manual.nextron-systems.com/en/latest/administration/api.html\nsummary: The published THOR Thunderstorm OpenAPI declares no securitySchemes and the THOR manual documents unauthenticated calls (curl -X POST \"http://myserver:8080/api/check?source=test\" -F \"file=@sample.exe\"); access control is the customer's network placement of the self-hosted service. The Analysis Cockpit API uses a per-user API key (\"copy the API key from your user settings into the key field\"). ASGARD license issuance uses a download token passed as a token query parameter.\nschemes:\n- name: none\n  type: none\n  api: nextron-systems:thor-thunderstorm-api\n  description: No authentication declared in the contract; self-hosted service on the customer's network.\n  sources:\n  - openapi/nextron-systems-thunderstorm-openapi.yml\n  - https://thor-manual.nextron-systems.com/en/latest/usage/deployment.html\n- name: Analysis Cockpit\
  \ API key\n  type: apiKey\n  api: nextron-systems:analysis-cockpit-api\n  description: To test the API in the web interface, copy the API key from your user settings into the key field. Header/parameter name is not published outside the appliance.\n  sources:\n  - https://analysis-cockpit-manual.nextron-systems.com/en/latest/administration/api.html\n- name: ASGARD download token\n  type: apiKey\n  in: query\n  parameter: token\n  api: nextron-systems:asgard-management-center-api\n  description: 'Licensing endpoint example: curl -XPOST \"https://my-asgard.internal:8443/api/v0/licensing/issue?token=...\" (download token configured under Downloads > Download Token Configuration).'\n  sources:\n  - https://thor-manual.nextron-systems.com/en/latest/usage/deployment.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextron-systems/refs/heads/main/authentication/nextron-systems-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Cybersecurity
- Forensics
- Compromise Assessment
- Threat Detection
- Malware Analysis
- Incident Response
---
