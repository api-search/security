---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: NetApp Cloud Manager API
  slug: netapp-cloud-manager-api
  spec_type: OpenAPI
  url: https://docs.netapp.com/us-en/cloud-manager-automation/api/openapi.yaml
- filename: netapp-ontap-openapi.yml
  format: yaml
  label: NetApp ONTAP REST API
  slug: netapp-ontap-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/openapi/netapp-ontap-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Netapp Authentication
name_suffix: Authentication
oauth_flows: []
overview: NetApp secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NetApp
provider_slug: netapp
scheme_count: 2
schemes:
- description: HTTP basic authentication using ONTAP user credentials. Provide the cluster or SVM administrator username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/netapp-ontap-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 bearer token authentication. Supported in ONTAP 9.8 and later.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/netapp-ontap-openapi.yml
  type: http
slug: netapp-authentication
source_filename: netapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/netapp-ontap-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP basic authentication using ONTAP user credentials. Provide the cluster or\n    SVM administrator username and password.\n  sources:\n  - openapi/netapp-ontap-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token authentication. Supported in ONTAP 9.8 and later.\n  sources:\n  - openapi/netapp-ontap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/authentication/netapp-authentication.yml
summary_line: http · 2 schemes
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
- Fortune 500
---
