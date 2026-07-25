---
api_key_in: []
api_specs:
- filename: microsoft-azure-traffic-manager-endpoints-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Endpoints API
  slug: microsoft-azure-traffic-manager-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-endpoints-api-openapi.yml
- filename: microsoft-azure-traffic-manager-geographichierarchies-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager GeographicHierarchies API
  slug: microsoft-azure-traffic-manager-geographichierarchies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-geographichierarchies-api-openapi.yml
- filename: microsoft-azure-traffic-manager-heatmap-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager HeatMap API
  slug: microsoft-azure-traffic-manager-heatmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-heatmap-api-openapi.yml
- filename: microsoft-azure-traffic-manager-profiles-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Profiles API
  slug: microsoft-azure-traffic-manager-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-profiles-api-openapi.yml
- filename: microsoft-azure-traffic-manager-usermetrics-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager UserMetrics API
  slug: microsoft-azure-traffic-manager-usermetrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-usermetrics-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Traffic Manager Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Traffic Manager secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Traffic Manager
provider_slug: microsoft-azure-traffic-manager
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-traffic-manager-openapi.yml
  type: oauth2
slug: microsoft-azure-traffic-manager-authentication
source_filename: microsoft-azure-traffic-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-traffic-manager-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth 2.0\n  sources:\n  - openapi/microsoft-azure-traffic-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/authentication/microsoft-azure-traffic-manager-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- DNS Load Balancing
- Failover
- Global Routing
- Networking
- Traffic Distribution
- Traffic Manager
---
