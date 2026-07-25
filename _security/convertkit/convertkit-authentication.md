---
api_key_in:
- header
api_specs:
- filename: convertkit-accounts-api-openapi.yml
  format: yaml
  label: Kit Accounts API
  slug: convertkit-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-accounts-api-openapi.yml
- filename: convertkit-broadcasts-api-openapi.yml
  format: yaml
  label: Kit Broadcasts API
  slug: convertkit-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-broadcasts-api-openapi.yml
- filename: convertkit-custom-fields-api-openapi.yml
  format: yaml
  label: Kit Custom Fields API
  slug: convertkit-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-custom-fields-api-openapi.yml
- filename: convertkit-email-templates-api-openapi.yml
  format: yaml
  label: Kit Email Templates API
  slug: convertkit-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-email-templates-api-openapi.yml
- filename: convertkit-forms-api-openapi.yml
  format: yaml
  label: Kit Forms API
  slug: convertkit-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-forms-api-openapi.yml
- filename: convertkit-posts-api-openapi.yml
  format: yaml
  label: Kit Posts API
  slug: convertkit-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-posts-api-openapi.yml
- filename: convertkit-purchases-api-openapi.yml
  format: yaml
  label: Kit Purchases API
  slug: convertkit-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-purchases-api-openapi.yml
- filename: convertkit-segments-api-openapi.yml
  format: yaml
  label: Kit Segments API
  slug: convertkit-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-segments-api-openapi.yml
- filename: convertkit-sequence-emails-api-openapi.yml
  format: yaml
  label: Kit Sequence Emails API
  slug: convertkit-sequence-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequence-emails-api-openapi.yml
- filename: convertkit-sequences-api-openapi.yml
  format: yaml
  label: Kit Sequences API
  slug: convertkit-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequences-api-openapi.yml
- filename: convertkit-snippets-api-openapi.yml
  format: yaml
  label: Kit Snippets API
  slug: convertkit-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-snippets-api-openapi.yml
- filename: convertkit-subscribers-api-openapi.yml
  format: yaml
  label: Kit Subscribers API
  slug: convertkit-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-subscribers-api-openapi.yml
- filename: convertkit-tags-api-openapi.yml
  format: yaml
  label: Kit Tags API
  slug: convertkit-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-tags-api-openapi.yml
- filename: convertkit-webhooks-api-openapi.yml
  format: yaml
  label: Kit Webhooks API
  slug: convertkit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Convertkit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kit secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kit
provider_slug: convertkit
scheme_count: 2
schemes:
- description: Authenticate API requests via an API Key
  in: header
  name: API Key
  parameter: X-Kit-Api-Key
  sources:
  - openapi/openapi.json
  type: apiKey
- description: Authenticate API requests via an OAuth token
  flows:
  - authorizationUrl: https://api.kit.com/v4/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.kit.com/v4/oauth/token
  name: OAuth2
  sources:
  - openapi/openapi.json
  type: oauth2
slug: convertkit-authentication
source_filename: convertkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: X-Kit-Api-Key\n  description: Authenticate API requests via an API Key\n  sources:\n  - openapi/openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kit.com/v4/oauth/authorize\n    tokenUrl: https://api.kit.com/v4/oauth/token\n    scopes: 2\n  description: Authenticate API requests via an OAuth token\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/authentication/convertkit-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Email Marketing
- Creator Economy
- Subscribers
- Automation
- Newsletters
- Sequences
- Forms
- Broadcasts
---
