---
api_key_in: []
api_specs:
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Registry API
  slug: benchling-lims-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Sequences API
  slug: benchling-lims-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Inventory API
  slug: benchling-lims-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Notebook (Entries) API
  slug: benchling-lims-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Assay Results & Runs API
  slug: benchling-lims-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Workflows API
  slug: benchling-lims-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Requests API
  slug: benchling-lims-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Events API
  slug: benchling-lims-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Apps & Webhooks API
  slug: benchling-lims-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Organizations & Users API
  slug: benchling-lims-org-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Blobs & Files API
  slug: benchling-lims-blobs-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Benchling Lims Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Benchling secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Benchling
provider_slug: benchling-lims
scheme_count: 2
schemes:
- description: 'Personal user API key sent as HTTP Basic auth (Authorization: Basic {api_key}). Generate a key on your Benchling user settings page.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/benchling-lims-openapi.yml
  type: http
- description: Benchling Apps authenticate with OAuth2 client credentials. Exchange client_id/client_secret at POST /api/v2/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{tenant}.benchling.com/api/v2/token
  name: appBearerAuth
  sources:
  - openapi/benchling-lims-openapi.yml
  type: oauth2
slug: benchling-lims-authentication
source_filename: benchling-lims-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/benchling-lims-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Personal user API key sent as HTTP Basic auth (Authorization: Basic {api_key}).\n    Generate a key on your Benchling user settings page.'\n  sources:\n  - openapi/benchling-lims-openapi.yml\n- name: appBearerAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.benchling.com/api/v2/token\n    scopes: 0\n  description: Benchling Apps authenticate with OAuth2 client credentials. Exchange client_id/client_secret\n    at POST /api/v2/token for a Bearer access_token.\n  sources:\n  - openapi/benchling-lims-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/authentication/benchling-lims-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Life Sciences
- Biotech
- LIMS
- Electronic Lab Notebook
- Registry
- Molecular Biology
- Inventory Management
- Assay Management
- Workflows
- Webhooks
- REST
---
