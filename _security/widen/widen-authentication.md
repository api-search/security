---
api_key_in: []
api_specs:
- filename: widen-acquia-dam-webhooks-api-openapi.yml
  format: yaml
  label: Widen Acquia-DAM-Webhooks API
  slug: widen-acquia-dam-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-acquia-dam-webhooks-api-openapi.yml
- filename: widen-analytics-api-openapi.yml
  format: yaml
  label: Widen Analytics API
  slug: widen-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-analytics-api-openapi.yml
- filename: widen-assets-api-openapi.yml
  format: yaml
  label: Widen Assets API
  slug: widen-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-assets-api-openapi.yml
- filename: widen-attributes-api-openapi.yml
  format: yaml
  label: Widen Attributes API
  slug: widen-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-attributes-api-openapi.yml
- filename: widen-categories-api-openapi.yml
  format: yaml
  label: Widen Categories API
  slug: widen-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-categories-api-openapi.yml
- filename: widen-channels-api-openapi.yml
  format: yaml
  label: Widen Channels API
  slug: widen-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-channels-api-openapi.yml
- filename: widen-collections-api-openapi.yml
  format: yaml
  label: Widen Collections API
  slug: widen-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-collections-api-openapi.yml
- filename: widen-file-formats-api-openapi.yml
  format: yaml
  label: Widen File-Formats API
  slug: widen-file-formats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-file-formats-api-openapi.yml
- filename: widen-integration-links-api-openapi.yml
  format: yaml
  label: Widen Integration-Links API
  slug: widen-integration-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-integration-links-api-openapi.yml
- filename: widen-metadata-api-openapi.yml
  format: yaml
  label: Widen Metadata API
  slug: widen-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-metadata-api-openapi.yml
- filename: widen-orders-api-openapi.yml
  format: yaml
  label: Widen Orders API
  slug: widen-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-orders-api-openapi.yml
- filename: widen-products-api-openapi.yml
  format: yaml
  label: Widen Products API
  slug: widen-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-products-api-openapi.yml
- filename: widen-search-connector-api-openapi.yml
  format: yaml
  label: Widen Search-Connector API
  slug: widen-search-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-search-connector-api-openapi.yml
- filename: widen-usage-api-openapi.yml
  format: yaml
  label: Widen Usage API
  slug: widen-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-usage-api-openapi.yml
- filename: widen-users-api-openapi.yml
  format: yaml
  label: Widen Users API
  slug: widen-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-users-api-openapi.yml
- filename: widen-workflow-app-projects-api-openapi.yml
  format: yaml
  label: Widen Workflow-App-Projects API
  slug: widen-workflow-app-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-workflow-app-projects-api-openapi.yml
- filename: widen-workflow-webhooks-api-openapi.yml
  format: yaml
  label: Widen Workflow-Webhooks API
  slug: widen-workflow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-workflow-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Widen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Widen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Widen
provider_slug: widen
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 Bearer token obtained from Acquia DAM.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: widen-authentication
source_filename: widen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 Bearer token obtained from Acquia DAM.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/authentication/widen-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Asset Management
- DAM
- Media
- Assets
- Metadata
- Collections
- Workflows
- Acquia
---
