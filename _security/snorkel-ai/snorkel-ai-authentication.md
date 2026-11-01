---
anonymous_access: false
api_key_in:
- sdk-context
api_specs:
- filename: snorkel-ai-openapi-generated.yml
  format: yaml
  label: Snorkel Platform REST API
  slug: snorkel-platform-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snorkel-ai/openapi/_ae-authored/snorkel-ai-openapi-generated.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Snorkel Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snorkel AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snorkel AI
provider_slug: snorkel-ai
scheme_count: 1
schemes:
- description: 'Per-user API key generated in User settings > API Keys. Docs: "API Keys can act as a replacement for your username and password when using the SDK or API." "Your API Key will only be shown in full once. Currently only a single API key can be active per user." Keys can be revoked from the same page. The SDK passes the key via SnorkelSDKContext.from_endpoint_url(endpoint, api_key, workspace_name) against the customer''s own instance host (https://<your-snorkel-hostname>). The HTTP header carrying the key is not documented.'
  key_count_per_user: 1
  name: apiKey
  revocable: true
  type: apiKey
slug: snorkel-ai-authentication
source_filename: snorkel-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource: https://docs.snorkel.ai/docs/26.7/administration/settings-and-administration/user-and-admin-settings\ndocs: https://docs.snorkel.ai/docs/26.7/administration/settings-and-administration/user-and-admin-settings#generating-and-using-api-keys\nx-docs-more:\n- https://docs.snorkel.ai/docs/26.7/administration/authentication/platform-authentication-and-user-roles\n- https://docs.snorkel.ai/docs/26.7/user-guide/sdk/quick_start/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - sdk-context\nschemes:\n- name: apiKey\n  type: apiKey\n  description: 'Per-user API key generated in User settings > API Keys. Docs: \"API Keys can act as a replacement for your username and password when using the SDK or API.\" \"Your API Key will only be shown in full once. Currently only a single API key can be active per user.\" Keys can be revoked from the same page. The SDK passes the key via SnorkelSDKContext.from_endpoint_url(endpoint, api_key, workspace_name)\
  \ against the customer''s own instance host (https://<your-snorkel-hostname>). The HTTP header carrying the key is not documented.'\n  key_count_per_user: 1\n  revocable: true\nplatform_login:\n  note: 'Interactive (UI) login supports \"Basic authentication\" (username/password, the default on a fresh install) and SSO via SAML or OIDC, which the docs call \"the recommended authentication method\". These are user-login methods for the platform, not API auth schemes.'\n  sso:\n  - https://docs.snorkel.ai/docs/26.7/administration/authentication/configure-saml-sso\n  - https://docs.snorkel.ai/docs/26.7/administration/authentication/configure-oidc-sso\nauthorization:\n  model: workspace-scoped RBAC roles\n  roles: [Superadmin/System Admin, Admin/Workspace Admin, Developer, Reviewer, Annotator]\n  docs: https://docs.snorkel.ai/docs/26.7/administration/authentication/user-roles-definition\n"
source_yaml_url: https://artifacts.apis.io/snorkel-ai/authentication/snorkel-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Data Development
- Programmatic Labeling
- Weak Supervision
- Evaluation
- SDK
---
