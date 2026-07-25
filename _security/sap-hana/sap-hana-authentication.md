---
api_key_in: []
api_specs:
- filename: sap-hana-alerts-api-openapi.yml
  format: yaml
  label: SAP HANA Alerts API
  slug: sap-hana-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-alerts-api-openapi.yml
- filename: sap-hana-instance-mappings-api-openapi.yml
  format: yaml
  label: SAP HANA Instance Mappings API
  slug: sap-hana-instance-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-instance-mappings-api-openapi.yml
- filename: sap-hana-instances-api-openapi.yml
  format: yaml
  label: SAP HANA Instances API
  slug: sap-hana-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-instances-api-openapi.yml
- filename: sap-hana-metering-api-openapi.yml
  format: yaml
  label: SAP HANA Metering API
  slug: sap-hana-metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-metering-api-openapi.yml
- filename: sap-hana-metrics-api-openapi.yml
  format: yaml
  label: SAP HANA Metrics API
  slug: sap-hana-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-metrics-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Hana Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP HANA secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP HANA
provider_slug: sap-hana
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication using SAP Business Technology Platform credentials. Obtain an access token using client credentials flow with the UAA service URL, client ID, and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately 1799 seconds (30 minutes) and must be refreshed.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  sources:
  - openapi/sap-hana-cloud-rest-api.yml
  type: oauth2
slug: sap-hana-authentication
source_filename: sap-hana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-hana-cloud-rest-api.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authentication using SAP Business Technology Platform credentials.\n    Obtain an access token using client credentials flow with the UAA service URL, client ID,\n    and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately\n    1799 seconds (30 minutes) and must be refreshed.\n  sources:\n  - openapi/sap-hana-cloud-rest-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/authentication/sap-hana-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
---
