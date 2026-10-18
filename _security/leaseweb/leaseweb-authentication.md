---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leaseweb-abuse-api-openapi.yml
  format: yaml
  label: Leaseweb Abuse API
  slug: leaseweb-abuse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-abuse-api-openapi.yml
- filename: leaseweb-aggregationpack-api-openapi.yml
  format: yaml
  label: Leaseweb Aggregationpack API
  slug: leaseweb-aggregationpack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-aggregationpack-api-openapi.yml
- filename: leaseweb-dedicatedserver-api-openapi.yml
  format: yaml
  label: Leaseweb Dedicatedserver API
  slug: leaseweb-dedicatedserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-dedicatedserver-api-openapi.yml
- filename: leaseweb-dns-api-openapi.yml
  format: yaml
  label: Leaseweb Dns API
  slug: leaseweb-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-dns-api-openapi.yml
- filename: leaseweb-invoice-api-openapi.yml
  format: yaml
  label: Leaseweb Invoice API
  slug: leaseweb-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-invoice-api-openapi.yml
- filename: leaseweb-ipmgmt-api-openapi.yml
  format: yaml
  label: Leaseweb Ipmgmt API
  slug: leaseweb-ipmgmt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-ipmgmt-api-openapi.yml
- filename: leaseweb-networkequipment-api-openapi.yml
  format: yaml
  label: Leaseweb Networkequipment API
  slug: leaseweb-networkequipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-networkequipment-api-openapi.yml
- filename: leaseweb-objectstorage-api-openapi.yml
  format: yaml
  label: Leaseweb Objectstorage API
  slug: leaseweb-objectstorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-objectstorage-api-openapi.yml
- filename: leaseweb-ordering-api-openapi.yml
  format: yaml
  label: Leaseweb Ordering API
  slug: leaseweb-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/openapi/leaseweb-ordering-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Leaseweb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leaseweb declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Leaseweb
provider_slug: leaseweb
scheme_count: 2
schemes:
- description: Authentication for the APIs is required. To authenticate your call, you will need to sent your API key as X-LSW-Auth header. You can generate API keys in the Customer Portal.
  in: header
  key_management: https://secure.leaseweb.com/api-client-management/
  name: X-LSW-Auth
  parameter: X-LSW-Auth
  type: apiKey
- description: Declared as a securityScheme in every Leaseweb OpenAPI definition.
  name: BearerAuth
  scheme: bearer
  type: http
slug: leaseweb-authentication
source_filename: leaseweb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://developer.leaseweb.com/docs/\ndocs: https://developer.leaseweb.com/docs/\nschemes:\n- name: X-LSW-Auth\n  type: apiKey\n  in: header\n  parameter: X-LSW-Auth\n  description: \"Authentication for the APIs is required. To authenticate your call, you will need to sent your API key as X-LSW-Auth header. You can generate API keys in the Customer Portal.\"\n  key_management: https://secure.leaseweb.com/api-client-management/\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Declared as a securityScheme in every Leaseweb OpenAPI definition.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaseweb/refs/heads/main/authentication/leaseweb-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cloud
- Infrastructure-as-a-Service
- Bare Metal
- Dedicated Servers
- Object Storage
- DNS
- Hosting
---
