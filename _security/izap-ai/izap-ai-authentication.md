---
anonymous_access: false
api_key_in: []
api_specs:
- filename: izap-ai-api-tokens-api-openapi.yml
  format: yaml
  label: iZap.ai API Tokens API
  slug: izap-ai-api-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-api-tokens-api-openapi.yml
- filename: izap-ai-business-library-api-openapi.yml
  format: yaml
  label: iZap.ai Business Library API
  slug: izap-ai-business-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-business-library-api-openapi.yml
- filename: izap-ai-businesses-api-openapi.yml
  format: yaml
  label: iZap.ai Businesses API
  slug: izap-ai-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-businesses-api-openapi.yml
- filename: izap-ai-chats-api-openapi.yml
  format: yaml
  label: iZap.ai Chats API
  slug: izap-ai-chats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-chats-api-openapi.yml
- filename: izap-ai-contacts-api-openapi.yml
  format: yaml
  label: iZap.ai Contacts API
  slug: izap-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-contacts-api-openapi.yml
- filename: izap-ai-menus-api-openapi.yml
  format: yaml
  label: iZap.ai Menus API
  slug: izap-ai-menus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-menus-api-openapi.yml
- filename: izap-ai-messages-api-openapi.yml
  format: yaml
  label: iZap.ai Messages API
  slug: izap-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-messages-api-openapi.yml
- filename: izap-ai-transmissions-api-openapi.yml
  format: yaml
  label: iZap.ai Transmissions API
  slug: izap-ai-transmissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-transmissions-api-openapi.yml
- filename: izap-ai-webhooks-api-openapi.yml
  format: yaml
  label: iZap.ai Webhooks API
  slug: izap-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-webhooks-api-openapi.yml
- filename: izap-ai-whatsapp-cloud-api-openapi.yml
  format: yaml
  label: iZap.ai Whatsapp Cloud API
  slug: izap-ai-whatsapp-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-whatsapp-cloud-api-openapi.yml
- filename: izap-ai-whatsapp-templates-api-openapi.yml
  format: yaml
  label: iZap.ai Whatsapp Templates API
  slug: izap-ai-whatsapp-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/izap-ai/openapi/izap-ai-whatsapp-templates-api-openapi.yml
auth_types: []
description: Authentication methods for iZap API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: iZap.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: iZap.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: iZap.ai
provider_slug: izap-ai
scheme_count: 2
schemes:
- evidence: The REST API accepts a personal access token as a Bearer credential on every request.
  header: Authorization
  how_to_obtain: 'Create one from the dashboard: User Settings → API Keys.'
  location: header
  name: Personal Access Token
  type: http-bearer
- authorize_url: /oauth/authorize
  evidence: Use the authorization-code + PKCE flow for clients that act on behalf of a user.
  header: Authorization
  how_to_obtain: Public clients may self‑register via POST /oauth/register.
  location: header
  name: OAuth 2.0 (authorization code + PKCE)
  token_url: /oauth/token
  type: oauth2
slug: izap-ai-authentication
source_filename: izap-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://devs.izap.ai/en/api-reference/authentication.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://devs.izap.ai/en/api-reference/authentication.md\nsources:\n- https://devs.izap.ai/en/api-reference/authentication.md\n- https://devs.izap.ai/en/quickstart.md\n- https://devs.izap.ai/en/api-reference/wizard.md\ndescription: Authentication methods for iZap API\nschemes:\n- type: http-bearer\n  name: Personal Access Token\n  evidence: The REST API accepts a personal access token as a Bearer credential on every request.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create one from the dashboard: User Settings → API Keys.'\n- type: oauth2\n  name: OAuth 2.0 (authorization code + PKCE)\n  evidence: Use the authorization-code + PKCE flow for clients that act on behalf of a user.\n  location: header\n  header: Authorization\n  token_url: /oauth/token\n  authorize_url: /oauth/authorize\n  how_to_obtain: Public clients may self‑register via POST /oauth/register.\n\
  docs: https://devs.izap.ai/en/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/izap-ai/authentication/izap-ai-authentication.yml
summary_line: 2 schemes
tags:
- WhatsApp
- Restaurant
---
