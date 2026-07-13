---
api_key_in:
- cookie
api_specs:
- filename: sap-business-one-service-layer-openapi.yml
  format: yaml
  label: SAP Business One Service Layer API
  slug: sap-business-one-service-layer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-business-one-service-layer-openapi.yml
- filename: sap-s4hana-cloud-business-partner-openapi.yml
  format: yaml
  label: SAP S/4HANA Cloud API
  slug: sap-s4hana-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-s4hana-cloud-business-partner-openapi.yml
- filename: sap-event-mesh-asyncapi.yml
  format: yaml
  label: SAP Event Mesh API
  slug: sap-event-mesh-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/asyncapi/sap-event-mesh-asyncapi.yml
- filename: sap-ai-core-openapi.yml
  format: yaml
  label: SAP AI Core API
  slug: sap-ai-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-ai-core-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP
provider_slug: sap
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  sources:
  - openapi/sap-ai-core-openapi.yml
  - openapi/sap-s4hana-cloud-business-partner-openapi.yml
  type: oauth2
- description: Session cookie obtained from the Login endpoint
  in: cookie
  name: sessionCookie
  parameter: B1SESSION
  sources:
  - openapi/sap-business-one-service-layer-openapi.yml
  type: apiKey
- description: Basic authentication with SAP user credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sap-s4hana-cloud-business-partner-openapi.yml
  type: http
slug: sap-authentication
source_filename: sap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-ai-core-openapi.yml, openapi/sap-business-one-service-layer-openapi.yml,\n  openapi/sap-s4hana-cloud-business-partner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/sap-ai-core-openapi.yml\n  - openapi/sap-s4hana-cloud-business-partner-openapi.yml\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: B1SESSION\n  description: Session cookie obtained from the Login endpoint\n  sources:\n  - openapi/sap-business-one-service-layer-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with SAP user credentials\n  sources:\n  - openapi/sap-s4hana-cloud-business-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/authentication/sap-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
---
