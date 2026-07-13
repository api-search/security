---
api_key_in: []
api_specs:
- filename: search-category.yaml
  format: yaml
  label: Bloomreach Discovery API
  slug: bloomreach-discovery-api
  spec_type: OpenAPI
  url: https://github.com/bloomreach/api-specs/blob/main/discovery/search-category.yaml
- filename: catalog-management.yaml
  format: yaml
  label: Bloomreach Discovery Catalog Management API
  slug: bloomreach-discovery-catalog-management-api
  spec_type: OpenAPI
  url: https://github.com/bloomreach/api-specs/blob/main/discovery/catalog-management.yaml
- filename: workspace-import-api.yaml
  format: yaml
  label: Bloomreach Data Hub Workspace Import API
  slug: bloomreach-data-hub-workspace-import-api
  spec_type: OpenAPI
  url: https://github.com/bloomreach/api-specs/blob/main/data-hub/workspace-import-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bloomreach Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloomreach secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bloomreach
provider_slug: bloomreach
scheme_count: 2
schemes:
- description: 'HTTP Basic authentication using an API Key ID and API Secret.

    For this workspace-scoped endpoint, use a workspace API key.


    `Authorization: Basic <base64(APIKeyID:APISecret)>`


    The API key must have the **Imports → Allow trigger imports**

    permission enabled in Workspace settings → Access management →

    API.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bloomreach-data-hub-workspace-import-openapi.yml
  type: http
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bloomreach-discovery-catalog-management-openapi.yml
  type: http
slug: bloomreach-authentication
source_filename: bloomreach-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloomreach-data-hub-workspace-import-openapi.yml, openapi/bloomreach-discovery-catalog-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic authentication using an API Key ID and API Secret.\n    For this workspace-scoped endpoint, use a workspace API key.\n\n    `Authorization: Basic <base64(APIKeyID:APISecret)>`\n\n    The API key must have the **Imports → Allow trigger imports**\n    permission enabled in Workspace settings → Access management →\n    API.\n  sources:\n  - openapi/bloomreach-data-hub-workspace-import-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/bloomreach-discovery-catalog-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomreach/refs/heads/main/authentication/bloomreach-authentication.yml
summary_line: http · 2 schemes
tags:
- Digital Commerce
- Search
- Merchandising
- Recommendations
- Customer Data Platform
- CDP
- Email Marketing
- SMS Marketing
- Marketing Automation
- Headless CMS
- Personalization
- E-commerce
---
