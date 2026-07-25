---
api_key_in:
- header
api_specs:
- filename: gencove-array-api-openapi.yml
  format: yaml
  label: Gencove array API
  slug: gencove-array-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-array-api-openapi.yml
- filename: gencove-basespace-api-openapi.yml
  format: yaml
  label: Gencove basespace API
  slug: gencove-basespace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-basespace-api-openapi.yml
- filename: gencove-batch-api-openapi.yml
  format: yaml
  label: Gencove batch API
  slug: gencove-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-batch-api-openapi.yml
- filename: gencove-billing-api-openapi.yml
  format: yaml
  label: Gencove billing API
  slug: gencove-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-billing-api-openapi.yml
- filename: gencove-explorer-api-openapi.yml
  format: yaml
  label: Gencove explorer API
  slug: gencove-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-explorer-api-openapi.yml
- filename: gencove-file-api-openapi.yml
  format: yaml
  label: Gencove file API
  slug: gencove-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-file-api-openapi.yml
- filename: gencove-firstmile-api-openapi.yml
  format: yaml
  label: Gencove firstmile API
  slug: gencove-firstmile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-firstmile-api-openapi.yml
- filename: gencove-invitation-api-openapi.yml
  format: yaml
  label: Gencove invitation API
  slug: gencove-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-invitation-api-openapi.yml
- filename: gencove-jwt-api-openapi.yml
  format: yaml
  label: Gencove jwt API
  slug: gencove-jwt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-jwt-api-openapi.yml
- filename: gencove-mfa-api-openapi.yml
  format: yaml
  label: Gencove mfa API
  slug: gencove-mfa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-mfa-api-openapi.yml
- filename: gencove-notification-api-openapi.yml
  format: yaml
  label: Gencove notification API
  slug: gencove-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-notification-api-openapi.yml
- filename: gencove-organization-api-openapi.yml
  format: yaml
  label: Gencove organization API
  slug: gencove-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-organization-api-openapi.yml
- filename: gencove-pipeline-api-openapi.yml
  format: yaml
  label: Gencove pipeline API
  slug: gencove-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-pipeline-api-openapi.yml
- filename: gencove-project-api-openapi.yml
  format: yaml
  label: Gencove project API
  slug: gencove-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-project-api-openapi.yml
- filename: gencove-role-api-openapi.yml
  format: yaml
  label: Gencove role API
  slug: gencove-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-role-api-openapi.yml
- filename: gencove-s3-api-openapi.yml
  format: yaml
  label: Gencove s3 API
  slug: gencove-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-s3-api-openapi.yml
- filename: gencove-sample-api-openapi.yml
  format: yaml
  label: Gencove sample API
  slug: gencove-sample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-sample-api-openapi.yml
- filename: gencove-social-api-openapi.yml
  format: yaml
  label: Gencove social API
  slug: gencove-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-social-api-openapi.yml
- filename: gencove-upload-api-openapi.yml
  format: yaml
  label: Gencove upload API
  slug: gencove-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-upload-api-openapi.yml
- filename: gencove-user-api-openapi.yml
  format: yaml
  label: Gencove user API
  slug: gencove-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gencove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gencove secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gencove
provider_slug: gencove
scheme_count: 2
schemes:
- description: 'Authorization header content formatted as: `Api-Key <API-key>`

    Obtain an API key through Gencove''s web UI (Account Settings -> API Keys)

    or the user-api-key endpoint.'
  docs: https://docs.gencove.com/base/getting-started/
  in: header
  name: API key
  parameter: Authorization
  scheme_hint: Api-Key <API-key>
  sources:
  - openapi/gencove-openapi-original.json
  type: apiKey
- description: 'Authorization header content formatted as: `Bearer <json-web-token>`

    Obtain an access token using the jwt-create endpoint; refresh via

    jwt-refresh and verify via jwt-verify.'
  in: header
  name: JWT
  parameter: Authorization
  scheme_hint: Bearer <json-web-token>
  sources:
  - openapi/gencove-openapi-original.json
  type: apiKey
slug: gencove-authentication
source_filename: gencove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/gencove-openapi-original.json\ndocs: https://docs.gencove.com/base/getting-started/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Gencove uses a static API key by default (Authorization: Api-Key <key>),\n    issued from the dashboard under Account Settings -> API Keys. A short-lived\n    JWT bearer token flow is also available via the jwt-create endpoint\n    (Authorization: Bearer <jwt>). Email/password env vars ($GENCOVE_EMAIL /\n    $GENCOVE_PASSWORD) can be used by the CLI to obtain a token but cannot be\n    combined with $GENCOVE_API_KEY.\nschemes:\n- name: API key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_hint: 'Api-Key <API-key>'\n  description: |-\n    Authorization header content formatted as: `Api-Key <API-key>`\n    Obtain an API key through Gencove's web UI (Account Settings -> API Keys)\n    or the user-api-key endpoint.\n  docs: https://docs.gencove.com/base/getting-started/\n\
  \  sources:\n  - openapi/gencove-openapi-original.json\n- name: JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_hint: 'Bearer <json-web-token>'\n  description: |-\n    Authorization header content formatted as: `Bearer <json-web-token>`\n    Obtain an access token using the jwt-create endpoint; refresh via\n    jwt-refresh and verify via jwt-verify.\n  sources:\n  - openapi/gencove-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/authentication/gencove-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Health
- Genomics
- Sequencing
- Bioinformatics
- DNA
- Life Sciences
- Analytics
---
