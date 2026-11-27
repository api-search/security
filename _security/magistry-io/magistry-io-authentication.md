---
anonymous_access: false
api_key_in: []
api_specs:
- filename: magistry-io-openapi-generated.yml
  format: yaml
  label: Magistry API
  slug: magistry-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magistry-io/openapi/_ae-authored/magistry-io-openapi-generated.yml
auth_types: []
description: Magistry supports API keys used as Bearer tokens and OAuth 2.1 flows.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Magistry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magistry declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Magistry
provider_slug: magistry-io
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer mag_sk_live_…'
  header: Authorization
  how_to_obtain: Create a key in Settings → Developers; keys are prefixed mag_sk_live_
  location: header
  name: API key (Bearer token)
  type: apiKey
- authorize_url: https://app.magistry.io/api/oauth/authorize
  evidence: '"bearer_methods_supported":["header"]"'
  flows:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:token-exchange
  how_to_obtain: Register a client via the registration endpoint https://app.magistry.io/api/oauth/register
  name: OAuth 2.1
  scopes:
  - read
  - write
  - catalog:read
  - catalog:write
  - ads:read
  - ads:write
  - analytics:read
  - analytics:write
  - merchant:read
  - merchant:write
  - orders:read
  - orders:write
  - cs:read
  - cs:write
  - promotions:read
  - promotions:write
  - costs:read
  - costs:write
  - automation:read
  - automation:write
  - research:read
  - research:write
  - reputation:read
  - reputation:write
  - disputes:read
  - disputes:write
  - creative:read
  - creative:write
  - finance:read
  - finance:write
  - theme:read
  - theme:write
  - social:read
  - social:write
  - settings:read
  - settings:write
  - integrations:read
  - integrations:write
  - developer:read
  - developer:write
  - billing:read
  - marketplaces:read
  - marketplaces:write
  - workspace:read
  - workspace:write
  - admin
  - offline_access
  type: oauth2
slug: magistry-io-authentication
source_filename: magistry-io-authentication.yml
source_heading: Authentication Profile
source_url: https://app.magistry.io/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.magistry.io/.well-known/oauth-protected-resource\nsources:\n- https://app.magistry.io/.well-known/oauth-protected-resource\n- https://app.magistry.io/.well-known/oauth-authorization-server\n- https://www.magistry.io/support/docs\n- https://www.magistry.io/support/help/api-keys-and-scopes\ndescription: Magistry supports API keys used as Bearer tokens and OAuth 2.1 flows.\nschemes:\n- type: apiKey\n  name: API key (Bearer token)\n  evidence: 'Authorization: Bearer mag_sk_live_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → Developers; keys are prefixed mag_sk_live_\n- type: oauth2\n  name: OAuth 2.1\n  evidence: '\"bearer_methods_supported\":[\"header\"]\"'\n  flows:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  authorize_url: https://app.magistry.io/api/oauth/authorize\n\
  \  scopes:\n  - read\n  - write\n  - catalog:read\n  - catalog:write\n  - ads:read\n  - ads:write\n  - analytics:read\n  - analytics:write\n  - merchant:read\n  - merchant:write\n  - orders:read\n  - orders:write\n  - cs:read\n  - cs:write\n  - promotions:read\n  - promotions:write\n  - costs:read\n  - costs:write\n  - automation:read\n  - automation:write\n  - research:read\n  - research:write\n  - reputation:read\n  - reputation:write\n  - disputes:read\n  - disputes:write\n  - creative:read\n  - creative:write\n  - finance:read\n  - finance:write\n  - theme:read\n  - theme:write\n  - social:read\n  - social:write\n  - settings:read\n  - settings:write\n  - integrations:read\n  - integrations:write\n  - developer:read\n  - developer:write\n  - billing:read\n  - marketplaces:read\n  - marketplaces:write\n  - workspace:read\n  - workspace:write\n  - admin\n  - offline_access\n  how_to_obtain: Register a client via the registration endpoint https://app.magistry.io/api/oauth/register\ndocs:\
  \ https://app.magistry.io/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/magistry-io/authentication/magistry-io-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Commerce
- Automation
- E-Commerce
- Netherlands
---
