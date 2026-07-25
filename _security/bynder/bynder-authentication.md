---
api_key_in: []
api_specs:
- filename: bynder-account-api-openapi.yml
  format: yaml
  label: Bynder Account API
  slug: bynder-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-account-api-openapi.yml
- filename: bynder-analytics-api-openapi.yml
  format: yaml
  label: Bynder Analytics API
  slug: bynder-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-analytics-api-openapi.yml
- filename: bynder-authentication-api-openapi.yml
  format: yaml
  label: Bynder Authentication API
  slug: bynder-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-authentication-api-openapi.yml
- filename: bynder-automation-api-openapi.yml
  format: yaml
  label: Bynder Automation API
  slug: bynder-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-automation-api-openapi.yml
- filename: bynder-brands-api-openapi.yml
  format: yaml
  label: Bynder Brands API
  slug: bynder-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-brands-api-openapi.yml
- filename: bynder-collections-api-openapi.yml
  format: yaml
  label: Bynder Collections API
  slug: bynder-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-collections-api-openapi.yml
- filename: bynder-contentaccess-api-openapi.yml
  format: yaml
  label: Bynder ContentAccess API
  slug: bynder-contentaccess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-contentaccess-api-openapi.yml
- filename: bynder-derivatives-api-openapi.yml
  format: yaml
  label: Bynder Derivatives API
  slug: bynder-derivatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-derivatives-api-openapi.yml
- filename: bynder-media-api-openapi.yml
  format: yaml
  label: Bynder Media API
  slug: bynder-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-media-api-openapi.yml
- filename: bynder-metaproperties-api-openapi.yml
  format: yaml
  label: Bynder Metaproperties API
  slug: bynder-metaproperties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-metaproperties-api-openapi.yml
- filename: bynder-orders-api-openapi.yml
  format: yaml
  label: Bynder Orders API
  slug: bynder-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-orders-api-openapi.yml
- filename: bynder-quarantine-api-openapi.yml
  format: yaml
  label: Bynder Quarantine API
  slug: bynder-quarantine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-quarantine-api-openapi.yml
- filename: bynder-smartfilters-api-openapi.yml
  format: yaml
  label: Bynder Smartfilters API
  slug: bynder-smartfilters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-smartfilters-api-openapi.yml
- filename: bynder-tags-api-openapi.yml
  format: yaml
  label: Bynder Tags API
  slug: bynder-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-tags-api-openapi.yml
- filename: bynder-taxonomy-api-openapi.yml
  format: yaml
  label: Bynder Taxonomy API
  slug: bynder-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-taxonomy-api-openapi.yml
- filename: bynder-trash-api-openapi.yml
  format: yaml
  label: Bynder Trash API
  slug: bynder-trash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-trash-api-openapi.yml
- filename: bynder-upload-api-openapi.yml
  format: yaml
  label: Bynder Upload API
  slug: bynder-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-upload-api-openapi.yml
- filename: bynder-users-api-openapi.yml
  format: yaml
  label: Bynder Users API
  slug: bynder-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-users-api-openapi.yml
- filename: bynder-webhooks-api-openapi.yml
  format: yaml
  label: Bynder Webhooks API
  slug: bynder-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-webhooks-api-openapi.yml
- filename: bynder-workflow-api-openapi.yml
  format: yaml
  label: Bynder Workflow API
  slug: bynder-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-workflow-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bynder Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Bynder secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Bynder
provider_slug: bynder
scheme_count: 1
schemes:
- description: OAuth 2.0 with JWT bearer access tokens
  flows:
  - authorizationUrl: https://yourportal.bynder.com/v6/authentication/oauth2/auth
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials
  name: oauth2
  sources:
  - openapi/bynder-openapi.yml
  type: oauth2
slug: bynder-authentication
source_filename: bynder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bynder-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://yourportal.bynder.com/v6/authentication/oauth2/auth\n    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization\n    scopes: 7\n  - flow: clientCredentials\n    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials\n    scopes: 2\n  description: OAuth 2.0 with JWT bearer access tokens\n  sources:\n  - openapi/bynder-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/authentication/bynder-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Digital Asset Management
- DAM
- Brand Management
- Content Management
- Marketing
---
