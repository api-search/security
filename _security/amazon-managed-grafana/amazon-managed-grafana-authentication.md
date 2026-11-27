---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-managed-grafana-tags-api-openapi.yml
  format: yaml
  label: Amazon Managed Grafana Tags API
  slug: amazon-managed-grafana-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-grafana/openapi/amazon-managed-grafana-tags-api-openapi.yml
- filename: amazon-managed-grafana-versions-api-openapi.yml
  format: yaml
  label: Amazon Managed Grafana Versions API
  slug: amazon-managed-grafana-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-grafana/openapi/amazon-managed-grafana-versions-api-openapi.yml
- filename: amazon-managed-grafana-workspaces-api-openapi.yml
  format: yaml
  label: Amazon Managed Grafana Workspaces API
  slug: amazon-managed-grafana-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-grafana/openapi/amazon-managed-grafana-workspaces-api-openapi.yml
- filename: amazon-managed-grafana-serviceaccounts-api-openapi.yml
  format: yaml
  label: Amazon Managed Grafana Managed Grafana Serviceaccounts API
  slug: amazon-managed-grafana-serviceaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-grafana/openapi/amazon-managed-grafana-serviceaccounts-api-openapi.yml
- filename: amazon-managed-grafana-tokens-api-openapi.yml
  format: yaml
  label: Amazon Managed Grafana Managed Grafana Tokens API
  slug: amazon-managed-grafana-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-grafana/openapi/amazon-managed-grafana-tokens-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Managed Grafana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Managed Grafana secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-managed-grafana-serviceaccounts-api-openapi.yml
  - openapi/amazon-managed-grafana-tags-api-openapi.yml
  - openapi/amazon-managed-grafana-tokens-api-openapi.yml
  - openapi/amazon-managed-grafana-versions-api-openapi.yml
  - openapi/amazon-managed-grafana-workspaces-api-openapi.yml
  type: apiKey
slug: amazon-managed-grafana-authentication
source_filename: amazon-managed-grafana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-managed-grafana-serviceaccounts-api-openapi.yml, openapi/amazon-managed-grafana-tags-api-openapi.yml,\n  openapi/amazon-managed-grafana-tokens-api-openapi.yml, openapi/amazon-managed-grafana-versions-api-openapi.yml,\n  openapi/amazon-managed-grafana-workspaces-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-managed-grafana-serviceaccounts-api-openapi.yml\n  - openapi/amazon-managed-grafana-tags-api-openapi.yml\n  - openapi/amazon-managed-grafana-tokens-api-openapi.yml\n  - openapi/amazon-managed-grafana-versions-api-openapi.yml\n  - openapi/amazon-managed-grafana-workspaces-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-managed-grafana/authentication/amazon-managed-grafana-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Dashboards
- Monitoring
- Observability
- Visualization
- Data Visualization
---
