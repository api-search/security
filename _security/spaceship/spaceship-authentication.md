---
api_key_in:
- header
api_specs:
- filename: spaceship-async-operations-api-openapi.yml
  format: yaml
  label: Spaceship Async Operations API
  slug: spaceship-async-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-async-operations-api-openapi.yml
- filename: spaceship-contacts-api-openapi.yml
  format: yaml
  label: Spaceship Contacts API
  slug: spaceship-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-contacts-api-openapi.yml
- filename: spaceship-contacts-attributes-api-openapi.yml
  format: yaml
  label: Spaceship Contacts attributes API
  slug: spaceship-contacts-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-contacts-attributes-api-openapi.yml
- filename: spaceship-dns-records-api-openapi.yml
  format: yaml
  label: Spaceship DNS records API
  slug: spaceship-dns-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-dns-records-api-openapi.yml
- filename: spaceship-domain-availability-api-openapi.yml
  format: yaml
  label: Spaceship Domain Availability API
  slug: spaceship-domain-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-domain-availability-api-openapi.yml
- filename: spaceship-domain-management-api-openapi.yml
  format: yaml
  label: Spaceship Domain Management API
  slug: spaceship-domain-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-domain-management-api-openapi.yml
- filename: spaceship-domain-settings-api-openapi.yml
  format: yaml
  label: Spaceship Domain Settings API
  slug: spaceship-domain-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-domain-settings-api-openapi.yml
- filename: spaceship-domain-transfer-api-openapi.yml
  format: yaml
  label: Spaceship Domain Transfer API
  slug: spaceship-domain-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-domain-transfer-api-openapi.yml
- filename: spaceship-personal-nameservers-api-openapi.yml
  format: yaml
  label: Spaceship Personal Nameservers API
  slug: spaceship-personal-nameservers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-personal-nameservers-api-openapi.yml
- filename: spaceship-sellerhub-api-openapi.yml
  format: yaml
  label: Spaceship SellerHub API
  slug: spaceship-sellerhub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-sellerhub-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spaceship Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spaceship secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spaceship
provider_slug: spaceship
scheme_count: 2
schemes:
- description: API key for authenticating requests, with a set of scopes (permissions) defined by the user at the time of creation.
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/spaceship-openapi-original.json
  type: apiKey
- description: API secret for authenticating requests must be set together with the API key.
  in: header
  name: apiSecret
  parameter: X-API-Secret
  sources:
  - openapi/spaceship-openapi-original.json
  type: apiKey
slug: spaceship-authentication
source_filename: spaceship-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/spaceship-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authenticating requests, with a set of scopes (permissions) defined\n    by the user at the time of creation.\n  sources:\n  - openapi/spaceship-openapi-original.json\n- name: apiSecret\n  type: apiKey\n  in: header\n  parameter: X-API-Secret\n  description: API secret for authenticating requests must be set together with the API key.\n  sources:\n  - openapi/spaceship-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/authentication/spaceship-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Domains
- Domain Registrar
- DNS
- Domain Marketplace
- Nameservers
- WHOIS
- Developer Tools
- API
---
