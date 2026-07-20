---
api_key_in:
- header
api_specs:
- filename: klaus-public-export-api-openapi-original.json
  format: json
  label: Klaus Public Export API
  slug: public-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaus/refs/heads/main/openapi/klaus-public-export-api-openapi-original.json
- filename: klaus-public-import-api-openapi-original.json
  format: json
  label: Klaus Public Import API
  slug: public-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaus/refs/heads/main/openapi/klaus-public-import-api-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Klaus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klaus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Klaus
provider_slug: klaus
scheme_count: 1
schemes:
- description: Enter the token with the "Bearer " prefix
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/klaus-public-export-api-openapi-original.json
  - openapi/klaus-public-import-api-openapi-original.json
  type: apiKey
slug: klaus-authentication
source_filename: klaus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/klaus-public-export-api-openapi-original.json, openapi/klaus-public-import-api-openapi-original.json\ndocs: https://support.zendesk.com/hc/en-us/articles/7043669282714-Setting-up-a-custom-integration-in-Zendesk-QA\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    A single bearer API token, issued per custom integration inside a Zendesk QA\n    account, is sent in the Authorization header as \"Bearer <api_token>\". There is\n    no OAuth 2.0 / OpenID Connect surface on the Klaus public APIs, and therefore no\n    scope model — access is bounded by the integration the token belongs to and by\n    the account/workspace identifiers supplied in the request.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Enter the token with the \"Bearer \" prefix\n  sources:\n  - openapi/klaus-public-export-api-openapi-original.json\n  - openapi/klaus-public-import-api-openapi-original.json\n\
  credentials:\n- name: API token\n  where: Zendesk QA > Settings > Account > Connections > custom integration\n  docs: https://support.zendesk.com/hc/en-us/articles/7043669282714-Setting-up-a-custom-integration-in-Zendesk-QA\n- name: account ID\n  where: Zendesk QA > Settings > Account > Connections > Edit connection\n  note: Required alongside the token for import/export requests.\n- name: workspace ID\n  where: Zendesk QA > Users, bots, and workspaces > Workspaces (the numeric id in the URL)\n  note: Required for the workspace-scoped export endpoints.\nnotes:\n- Export requests are made against the account's own Zendesk subdomain under the /qa\n  base path (for example https://yoursubdomain.zendesk.com/qa/api/export/reviews).\n- The Import API is additionally documented against the shared host\n  https://pub.klausapp.com/v1/tickets for non-migrated accounts.\n- 'Zendesk has removed password (basic) access for its APIs; token-based access is the\n  supported model. Reference:\n  https://support.zendesk.com/hc/en-us/articles/9941874259354-Deprecation-of-password-access-for-APIs'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaus/refs/heads/main/authentication/klaus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Quality Assurance
- Customer Support
- Customer Experience
- Conversation Analytics
- Contact Center
- Coaching
- Artificial Intelligence
- SaaS
---
