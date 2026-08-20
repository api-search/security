---
api_key_in:
- cookie
api_specs:
- filename: sap-event-mesh-asyncapi.yml
  format: yaml
  label: SAP Event Mesh API
  slug: sap-event-mesh-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/asyncapi/sap-event-mesh-asyncapi.yml
- filename: sap-addresses-api-openapi.yml
  format: yaml
  label: SAP Addresses API
  slug: sap-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-addresses-api-openapi.yml
- filename: sap-artifacts-api-openapi.yml
  format: yaml
  label: SAP Artifacts API
  slug: sap-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-artifacts-api-openapi.yml
- filename: sap-authentication-api-openapi.yml
  format: yaml
  label: SAP Authentication API
  slug: sap-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-authentication-api-openapi.yml
- filename: sap-bank-accounts-api-openapi.yml
  format: yaml
  label: SAP Bank Accounts API
  slug: sap-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-bank-accounts-api-openapi.yml
- filename: sap-business-partners-api-openapi.yml
  format: yaml
  label: SAP Business Partners API
  slug: sap-business-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-business-partners-api-openapi.yml
- filename: sap-configurations-api-openapi.yml
  format: yaml
  label: SAP Configurations API
  slug: sap-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-configurations-api-openapi.yml
- filename: sap-deployments-api-openapi.yml
  format: yaml
  label: SAP Deployments API
  slug: sap-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-deployments-api-openapi.yml
- filename: sap-executions-api-openapi.yml
  format: yaml
  label: SAP Executions API
  slug: sap-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-executions-api-openapi.yml
- filename: sap-invoices-api-openapi.yml
  format: yaml
  label: SAP Invoices API
  slug: sap-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-invoices-api-openapi.yml
- filename: sap-items-api-openapi.yml
  format: yaml
  label: SAP Items API
  slug: sap-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-items-api-openapi.yml
- filename: sap-journal-entries-api-openapi.yml
  format: yaml
  label: SAP Journal Entries API
  slug: sap-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-journal-entries-api-openapi.yml
- filename: sap-orders-api-openapi.yml
  format: yaml
  label: SAP Orders API
  slug: sap-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-orders-api-openapi.yml
- filename: sap-roles-api-openapi.yml
  format: yaml
  label: SAP Roles API
  slug: sap-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-roles-api-openapi.yml
- filename: sap-scenarios-api-openapi.yml
  format: yaml
  label: SAP Scenarios API
  slug: sap-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-scenarios-api-openapi.yml
- filename: sap-tax-numbers-api-openapi.yml
  format: yaml
  label: SAP Tax Numbers API
  slug: sap-tax-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-tax-numbers-api-openapi.yml
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
- Artificial Intelligence
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
---
