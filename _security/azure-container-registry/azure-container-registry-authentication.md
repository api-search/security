---
anonymous_access: false
api_key_in: []
api_specs:
- filename: azure-container-registry-registries-api-openapi.yml
  format: yaml
  label: Azure Container Registry Registries API
  slug: azure-container-registry-registries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-registries-api-openapi.yml
- filename: azure-container-registry-replications-api-openapi.yml
  format: yaml
  label: Azure Container Registry Replications API
  slug: azure-container-registry-replications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-replications-api-openapi.yml
- filename: azure-container-registry-webhooks-api-openapi.yml
  format: yaml
  label: Azure Container Registry Webhooks API
  slug: azure-container-registry-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-webhooks-api-openapi.yml
- filename: azure-container-registry-blobs-api-openapi.yml
  format: yaml
  label: Azure Container Registry Blobs API
  slug: microsoft-azure-container-registry-blobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-blobs-api-openapi.yml
- filename: azure-container-registry-manifests-api-openapi.yml
  format: yaml
  label: Azure Container Registry Manifests API
  slug: microsoft-azure-container-registry-manifests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-manifests-api-openapi.yml
- filename: azure-container-registry-acr-api-openapi.yml
  format: yaml
  label: Azure Container Registry Acr API
  slug: azure-container-registry-acr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-acr-api-openapi.yml
- filename: azure-container-registry-azure-container-registry-api-openapi.yml
  format: yaml
  label: Azure Container Registry Azure Container Registry API
  slug: azure-container-registry-azure-container-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-azure-container-registry-api-openapi.yml
- filename: azure-container-registry-cacherules-api-openapi.yml
  format: yaml
  label: Azure Container Registry Cache Rules API
  slug: azure-container-registry-cacherules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-cacherules-api-openapi.yml
- filename: azure-container-registry-connectedregistries-api-openapi.yml
  format: yaml
  label: Azure Container Registry Connected Registries API
  slug: azure-container-registry-connectedregistries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-connectedregistries-api-openapi.yml
- filename: azure-container-registry-credentialsets-api-openapi.yml
  format: yaml
  label: Azure Container Registry Credential Sets API
  slug: azure-container-registry-credentialsets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-credentialsets-api-openapi.yml
- filename: azure-container-registry-oauth2-api-openapi.yml
  format: yaml
  label: Azure Container Registry Oauth2 API
  slug: azure-container-registry-oauth2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-oauth2-api-openapi.yml
- filename: azure-container-registry-operations-api-openapi.yml
  format: yaml
  label: Azure Container Registry Operations API
  slug: azure-container-registry-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-operations-api-openapi.yml
- filename: azure-container-registry-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Container Registry Private Link Resources API
  slug: azure-container-registry-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-privatelinkresources-api-openapi.yml
- filename: azure-container-registry-runs-api-openapi.yml
  format: yaml
  label: Azure Container Registry Runs API
  slug: azure-container-registry-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-runs-api-openapi.yml
- filename: azure-container-registry-scopemaps-api-openapi.yml
  format: yaml
  label: Azure Container Registry Scope Maps API
  slug: azure-container-registry-scopemaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-scopemaps-api-openapi.yml
- filename: azure-container-registry-tasks-api-openapi.yml
  format: yaml
  label: Azure Container Registry Tasks API
  slug: azure-container-registry-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-tasks-api-openapi.yml
- filename: azure-container-registry-tokens-api-openapi.yml
  format: yaml
  label: Azure Container Registry Tokens API
  slug: azure-container-registry-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-tokens-api-openapi.yml
- filename: azure-container-registry-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Container Registry Private Endpoint Connections API
  slug: azure-container-registry-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-private-endpoint-connections-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Azure Container Registry Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Container Registry secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Container Registry
provider_slug: azure-container-registry
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_superseded/azure-container-registry-blobs-api-openapi.yml
  - openapi/_superseded/azure-container-registry-manifests-api-openapi.yml
  - openapi/_superseded/azure-container-registry-repositories-api-openapi.yml
  - openapi/_superseded/azure-container-registry-tags-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: OAuth2Auth
  sources:
  - openapi/azure-container-registry-data-plane-api-openapi.yml
  - openapi/azure-container-registry-management-api-openapi.yml
  - openapi/azure-container-registry-operation-api-openapi.yml
  - openapi/_superseded/azure-container-registry-registries-api-openapi.yml
  - openapi/_superseded/azure-container-registry-replications-api-openapi.yml
  - openapi/_superseded/azure-container-registry-webhooks-api-openapi.yml
  type: oauth2
slug: azure-container-registry-authentication
source_filename: azure-container-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/azure-container-registry-blobs-api-openapi.yml, openapi/azure-container-registry-data-plane-api-openapi.yml,\n  openapi/azure-container-registry-management-api-openapi.yml, openapi/_superseded/azure-container-registry-manifests-api-openapi.yml,\n  openapi/azure-container-registry-operation-api-openapi.yml, openapi/_superseded/azure-container-registry-registries-api-openapi.yml,\n  openapi/_superseded/azure-container-registry-replications-api-openapi.yml, openapi/_superseded/azure-container-registry-repositories-api-openapi.yml,\n  openapi/_superseded/azure-container-registry-tags-api-openapi.yml, openapi/_superseded/azure-container-registry-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/_superseded/azure-container-registry-blobs-api-openapi.yml\n  - openapi/_superseded/azure-container-registry-manifests-api-openapi.yml\n\
  \  - openapi/_superseded/azure-container-registry-repositories-api-openapi.yml\n  - openapi/_superseded/azure-container-registry-tags-api-openapi.yml\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/azure-container-registry-data-plane-api-openapi.yml\n  - openapi/azure-container-registry-management-api-openapi.yml\n  - openapi/azure-container-registry-operation-api-openapi.yml\n  - openapi/_superseded/azure-container-registry-registries-api-openapi.yml\n  - openapi/_superseded/azure-container-registry-replications-api-openapi.yml\n  - openapi/_superseded/azure-container-registry-webhooks-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/azure-container-registry/authentication/azure-container-registry-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Microsoft Azure
- Container Images
- Containers
- Docker
- Registry
---
