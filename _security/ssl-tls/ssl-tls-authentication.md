---
api_key_in:
- header
api_specs:
- filename: ssl-tls-certificates-api-openapi.yml
  format: yaml
  label: SSL/TLS Certificates API
  slug: ssl-tls-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssl-tls/refs/heads/main/openapi/ssl-tls-certificates-api-openapi.yml
- filename: ssl-tls-domains-api-openapi.yml
  format: yaml
  label: SSL/TLS Domains API
  slug: ssl-tls-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssl-tls/refs/heads/main/openapi/ssl-tls-domains-api-openapi.yml
- filename: ssl-tls-monitoring-api-openapi.yml
  format: yaml
  label: SSL/TLS Monitoring API
  slug: ssl-tls-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssl-tls/refs/heads/main/openapi/ssl-tls-monitoring-api-openapi.yml
- filename: ssl-tls-orders-api-openapi.yml
  format: yaml
  label: SSL/TLS Orders API
  slug: ssl-tls-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssl-tls/refs/heads/main/openapi/ssl-tls-orders-api-openapi.yml
- filename: ssl-tls-revocation-api-openapi.yml
  format: yaml
  label: SSL/TLS Revocation API
  slug: ssl-tls-revocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssl-tls/refs/heads/main/openapi/ssl-tls-revocation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ssl Tls Authentication
name_suffix: Authentication
oauth_flows: []
overview: SSL/TLS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SSL/TLS
provider_slug: ssl-tls
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/ssl-tls-certificate-management-openapi.yml
  type: apiKey
slug: ssl-tls-authentication
source_filename: ssl-tls-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ssl-tls-certificate-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/ssl-tls-certificate-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ssl-tls/refs/heads/main/authentication/ssl-tls-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- SSL/TLS
- TLS
- Certificates
- PKI
- Cryptography
- Certificate Authority
- HTTPS
---
