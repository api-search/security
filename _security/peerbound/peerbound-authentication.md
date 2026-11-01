---
anonymous_access: false
api_key_in: []
api_specs:
- filename: peerbound-activities-api-openapi.yml
  format: yaml
  label: Peerbound Activities API
  slug: peerbound-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-activities-api-openapi.yml
- filename: peerbound-moments-api-openapi.yml
  format: yaml
  label: Peerbound Moments API
  slug: peerbound-moments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-moments-api-openapi.yml
- filename: peerbound-notes-api-openapi.yml
  format: yaml
  label: Peerbound Notes API
  slug: peerbound-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-notes-api-openapi.yml
- filename: peerbound-reviews-api-openapi.yml
  format: yaml
  label: Peerbound Reviews API
  slug: peerbound-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-reviews-api-openapi.yml
- filename: peerbound-stories-api-openapi.yml
  format: yaml
  label: Peerbound Stories API
  slug: peerbound-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-stories-api-openapi.yml
auth_types: []
description: 'Peerbound supports two authentication methods for its MCP API: API key and OAuth 2.0.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Peerbound Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peerbound declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Peerbound
provider_slug: peerbound
scheme_count: 2
schemes:
- evidence: 'Include the key in the Authorization header: Authorization: Bearer <your-api-key>'
  header: Authorization
  how_to_obtain: Generate the API key from the Company Settings page at https://app.peerbound.com/settings/api-keys
  location: header
  name: API key
  type: apiKey
- evidence: 'Select your authentication method: OAuth 2.0 — recommended for individual users authenticating with their own Peerbound credentials'
  how_to_obtain: Users authenticate with their own Peerbound credentials through the OAuth flow provided by the integration (e.g., Claude, ChatGPT, Microsoft Copilot Studio).
  name: OAuth 2.0
  type: oauth2
slug: peerbound-authentication
source_filename: peerbound-authentication.yml
source_heading: Authentication Profile
source_url: https://help.peerbound.com/articles/3144479554-peerbound-onboarding-guide
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.peerbound.com/articles/3144479554-peerbound-onboarding-guide\nsources:\n- https://help.peerbound.com/articles/3144479554-peerbound-onboarding-guide\n- https://help.peerbound.com/articles/2744944512-peerbound-mcp-quick-start-guide\n- https://help.peerbound.com/articles/6227455949-peerbound-for-web-setup\n- https://help.peerbound.com/articles/9504680127-peerbound-for-web-setup-integrating-the-embed-code\ndescription: 'Peerbound supports two authentication methods for its MCP API: API key and OAuth 2.0.'\nschemes:\n- type: apiKey\n  name: API key\n  evidence: 'Include the key in the Authorization header: Authorization: Bearer <your-api-key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate the API key from the Company Settings page at https://app.peerbound.com/settings/api-keys\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'Select your authentication\
  \ method: OAuth 2.0 — recommended for individual users authenticating with their own Peerbound credentials'\n  how_to_obtain: Users authenticate with their own Peerbound credentials through the OAuth flow provided by the integration (e.g., Claude, ChatGPT,\n    Microsoft Copilot Studio).\ndocs: https://help.peerbound.com/articles/3144479554-peerbound-onboarding-guide\n"
source_yaml_url: https://artifacts.apis.io/peerbound/authentication/peerbound-authentication.yml
summary_line: 2 schemes
tags:
- Company
- SaaS
- Sales Enablement
- Customer Proof
- Analytics
---
