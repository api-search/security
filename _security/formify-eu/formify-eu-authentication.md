---
anonymous_access: false
api_key_in: []
api_specs:
- filename: formify-eu-account-api-openapi.yml
  format: yaml
  label: Formify Account API
  slug: formify-eu-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-account-api-openapi.yml
- filename: formify-eu-auth-api-openapi.yml
  format: yaml
  label: Formify Auth API
  slug: formify-eu-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-auth-api-openapi.yml
- filename: formify-eu-docs-api-openapi.yml
  format: yaml
  label: Formify Docs API
  slug: formify-eu-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-docs-api-openapi.yml
- filename: formify-eu-drafts-api-openapi.yml
  format: yaml
  label: Formify Drafts API
  slug: formify-eu-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-drafts-api-openapi.yml
- filename: formify-eu-files-api-openapi.yml
  format: yaml
  label: Formify Files API
  slug: formify-eu-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-files-api-openapi.yml
- filename: formify-eu-links-api-openapi.yml
  format: yaml
  label: Formify Links API
  slug: formify-eu-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-links-api-openapi.yml
- filename: formify-eu-oauth-api-openapi.yml
  format: yaml
  label: Formify OAuth API
  slug: formify-eu-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-oauth-api-openapi.yml
- filename: formify-eu-templates-api-openapi.yml
  format: yaml
  label: Formify Templates API
  slug: formify-eu-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-templates-api-openapi.yml
- filename: formify-eu-user-api-openapi.yml
  format: yaml
  label: Formify User API
  slug: formify-eu-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-user-api-openapi.yml
- filename: formify-eu-webhooks-api-openapi.yml
  format: yaml
  label: Formify Webhooks API
  slug: formify-eu-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-webhooks-api-openapi.yml
auth_types: []
description: Formify supports OAuth 2.0 Authorization Code flow and API‑key based bearer tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Formify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formify declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Formify
provider_slug: formify-eu
scheme_count: 1
schemes:
- evidence: 'If the AI client cannot complete OAuth for MCP servers: sign in to app.formify.eu , open Settings → Integration , create a clearly named API key, copy it, and configure it in the client as a token or as Authorization: Bearer sk_... .'
  header: Authorization
  how_to_obtain: 'Create an API key in Settings → Integration and use it as a Bearer token (e.g., "Authorization: Bearer sk_...").'
  location: header
  name: API key bearer token
  type: http-bearer
slug: formify-eu-authentication
source_filename: formify-eu-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.formify.eu/guides/oauth-for-ai/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.formify.eu/guides/oauth-for-ai/\nsources:\n- https://developers.formify.eu/guides/oauth-for-ai/\n- https://developers.formify.eu/#tag/oauth\n- https://developers.formify.eu/guides/oauth-for-ai/#option-b-dynamic-client-registration\n- https://developers.formify.eu/#tag/auth/operation/exchangeApiKeyForAccessToken\ndescription: Formify supports OAuth 2.0 Authorization Code flow and API‑key based bearer tokens.\nschemes:\n- type: http-bearer\n  name: API key bearer token\n  evidence: 'If the AI client cannot complete OAuth for MCP servers: sign in to app.formify.eu , open Settings → Integration , create a clearly\n    named API key, copy it, and configure it in the client as a token or as Authorization: Bearer sk_... .'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create an API key in Settings → Integration and use it as a Bearer token (e.g., \"\
  Authorization: Bearer sk_...\").'\ndocs: https://developers.formify.eu/guides/oauth-for-ai/\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/formify-eu/authentication/formify-eu-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- E-signing
- Legal Tech
- Multilingual
---
