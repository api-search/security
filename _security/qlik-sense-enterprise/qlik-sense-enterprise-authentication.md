---
api_key_in:
- header
api_specs:
- filename: qlik-sense-enterprise-repository-service-openapi.yml
  format: yaml
  label: Qlik Sense Repository Service
  slug: qlik-sense-repository-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-repository-service-openapi.yml
- filename: qlik-sense-enterprise-proxy-service-openapi.yml
  format: yaml
  label: Qlik Sense Proxy Service
  slug: qlik-sense-proxy-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-proxy-service-openapi.yml
- filename: qlik-sense-enterprise-about-service-openapi.yml
  format: yaml
  label: Qlik Sense About Service
  slug: qlik-sense-about-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-about-service-openapi.yml
- filename: qlik-sense-enterprise-data-connection-openapi.yml
  format: yaml
  label: Qlik Sense Data Connection
  slug: qlik-sense-data-connection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-data-connection-openapi.yml
- filename: qlik-sense-enterprise-licenses-openapi.yml
  format: yaml
  label: Qlik Sense Licenses
  slug: qlik-sense-licenses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-licenses-openapi.yml
- filename: qlik-sense-enterprise-odag-service-openapi.yml
  format: yaml
  label: Qlik Sense ODAG
  slug: qlik-sense-odag
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-odag-service-openapi.yml
auth_types:
- apiKey
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Qlik Sense Enterprise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qlik Sense Enterprise secures its APIs with apiKey, http, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
scheme_count: 3
schemes:
- description: Cross-site request forgery prevention key. Must be 16 arbitrary characters and must match the Xrfkey query parameter.
  in: header
  name: xrfkey
  parameter: X-Qlik-Xrfkey
  sources:
  - openapi/qlik-sense-enterprise-about-service-openapi.yml
  - openapi/qlik-sense-enterprise-data-connection-openapi.yml
  - openapi/qlik-sense-enterprise-licenses-openapi.yml
  - openapi/qlik-sense-enterprise-odag-service-openapi.yml
  - openapi/qlik-sense-enterprise-proxy-service-openapi.yml
  - openapi/qlik-sense-enterprise-repository-service-openapi.yml
  type: apiKey
- description: Client certificate authentication for direct QRS access on port 4242.
  name: certificate
  sources:
  - openapi/qlik-sense-enterprise-data-connection-openapi.yml
  - openapi/qlik-sense-enterprise-licenses-openapi.yml
  - openapi/qlik-sense-enterprise-proxy-service-openapi.yml
  - openapi/qlik-sense-enterprise-repository-service-openapi.yml
  type: mutualTLS
- description: Windows Integrated Authentication (NTLM/Kerberos) used when connecting via the Qlik Sense Proxy Service.
  name: windowsAuth
  scheme: negotiate
  sources:
  - openapi/qlik-sense-enterprise-repository-service-openapi.yml
  type: http
slug: qlik-sense-enterprise-authentication
source_filename: qlik-sense-enterprise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qlik-sense-enterprise-about-service-openapi.yml, openapi/qlik-sense-enterprise-data-connection-openapi.yml,\n  openapi/qlik-sense-enterprise-licenses-openapi.yml, openapi/qlik-sense-enterprise-odag-service-openapi.yml,\n  openapi/qlik-sense-enterprise-proxy-service-openapi.yml, openapi/qlik-sense-enterprise-repository-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - mutualTLS\n  api_key_in:\n  - header\nschemes:\n- name: xrfkey\n  type: apiKey\n  in: header\n  parameter: X-Qlik-Xrfkey\n  description: Cross-site request forgery prevention key. Must be 16 arbitrary characters and\n    must match the Xrfkey query parameter.\n  sources:\n  - openapi/qlik-sense-enterprise-about-service-openapi.yml\n  - openapi/qlik-sense-enterprise-data-connection-openapi.yml\n  - openapi/qlik-sense-enterprise-licenses-openapi.yml\n  - openapi/qlik-sense-enterprise-odag-service-openapi.yml\n  - openapi/qlik-sense-enterprise-proxy-service-openapi.yml\n\
  \  - openapi/qlik-sense-enterprise-repository-service-openapi.yml\n- name: certificate\n  type: mutualTLS\n  description: Client certificate authentication for direct QRS access on port 4242.\n  sources:\n  - openapi/qlik-sense-enterprise-data-connection-openapi.yml\n  - openapi/qlik-sense-enterprise-licenses-openapi.yml\n  - openapi/qlik-sense-enterprise-proxy-service-openapi.yml\n  - openapi/qlik-sense-enterprise-repository-service-openapi.yml\n- name: windowsAuth\n  type: http\n  scheme: negotiate\n  description: Windows Integrated Authentication (NTLM/Kerberos) used when connecting via the\n    Qlik Sense Proxy Service.\n  sources:\n  - openapi/qlik-sense-enterprise-repository-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/authentication/qlik-sense-enterprise-authentication.yml
summary_line: apiKey/http/mutualTLS · 3 schemes
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
---
