---
api_key_in: []
api_specs:
- filename: azure-health-collection-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Collection API
  slug: azure-health-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-collection-api-openapi.yml
- filename: azure-health-deid-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Deid API
  slug: azure-health-deid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-deid-api-openapi.yml
- filename: azure-health-dicomservices-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services DicomServices API
  slug: azure-health-dicomservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-dicomservices-api-openapi.yml
- filename: azure-health-fhirservices-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services FhirServices API
  slug: azure-health-fhirservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-fhirservices-api-openapi.yml
- filename: azure-health-iotconnectors-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services IotConnectors API
  slug: azure-health-iotconnectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-iotconnectors-api-openapi.yml
- filename: azure-health-jobs-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Jobs API
  slug: azure-health-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-jobs-api-openapi.yml
- filename: azure-health-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services PrivateEndpointConnections API
  slug: azure-health-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-privateendpointconnections-api-openapi.yml
- filename: azure-health-privatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services PrivateLinkResources API
  slug: azure-health-privatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-privatelinkresources-api-openapi.yml
- filename: azure-health-proxy-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Proxy API
  slug: azure-health-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-proxy-api-openapi.yml
- filename: azure-health-resource-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Resource API
  slug: azure-health-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-resource-api-openapi.yml
- filename: azure-health-workspaceprivateendpointconnections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services WorkspacePrivateEndpointConnections API
  slug: azure-health-workspaceprivateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaceprivateendpointconnections-api-openapi.yml
- filename: azure-health-workspaceprivatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services WorkspacePrivateLinkResources API
  slug: azure-health-workspaceprivatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaceprivatelinkresources-api-openapi.yml
- filename: azure-health-workspaces-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Workspaces API
  slug: azure-health-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaces-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Microsoft Azure Health Data Services secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Microsoft Azure Health Data Services
provider_slug: azure-health
scheme_count: 2
schemes:
- description: The Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: AadToken
  sources:
  - openapi/health-data-ai-deid-2024-11-15.json
  type: oauth2
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/healthcare-apis-2024-03-31.json
  type: oauth2
slug: azure-health-authentication
source_filename: azure-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/health-data-ai-deid-2024-11-15.json, openapi/healthcare-apis-2024-03-31.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: AadToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n    scopes: 1\n  description: The Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/health-data-ai-deid-2024-11-15.json\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/healthcare-apis-2024-03-31.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/authentication/azure-health-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Healthcare
- FHIR
- DICOM
- MedTech
- IoMT
- Health Data
- HIPAA
- HITRUST
- Cloud
- Azure
- Microsoft
---
