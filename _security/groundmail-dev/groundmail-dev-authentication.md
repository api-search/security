---
anonymous_access: false
api_key_in: []
api_specs:
- filename: groundmail-dev-automations-api-openapi.yml
  format: yaml
  label: groundmail-dev Automations API
  slug: groundmail-dev-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-automations-api-openapi.yml
- filename: groundmail-dev-deliverability-api-openapi.yml
  format: yaml
  label: groundmail-dev Deliverability API
  slug: groundmail-dev-deliverability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-deliverability-api-openapi.yml
- filename: groundmail-dev-dmarc-api-openapi.yml
  format: yaml
  label: groundmail-dev Dmarc API
  slug: groundmail-dev-dmarc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-dmarc-api-openapi.yml
- filename: groundmail-dev-domains-api-openapi.yml
  format: yaml
  label: groundmail-dev Domains API
  slug: groundmail-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-domains-api-openapi.yml
- filename: groundmail-dev-emails-api-openapi.yml
  format: yaml
  label: groundmail-dev Emails API
  slug: groundmail-dev-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-emails-api-openapi.yml
- filename: groundmail-dev-events-api-openapi.yml
  format: yaml
  label: groundmail-dev Events API
  slug: groundmail-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-events-api-openapi.yml
- filename: groundmail-dev-inbound-api-openapi.yml
  format: yaml
  label: groundmail-dev Inbound API
  slug: groundmail-dev-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-inbound-api-openapi.yml
- filename: groundmail-dev-integrations-api-openapi.yml
  format: yaml
  label: groundmail-dev Integrations API
  slug: groundmail-dev-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-integrations-api-openapi.yml
- filename: groundmail-dev-migrations-api-openapi.yml
  format: yaml
  label: groundmail-dev Migrations API
  slug: groundmail-dev-migrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-migrations-api-openapi.yml
- filename: groundmail-dev-oauth-api-openapi.yml
  format: yaml
  label: groundmail-dev OAuth API
  slug: groundmail-dev-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-oauth-api-openapi.yml
- filename: groundmail-dev-smtpcredentials-api-openapi.yml
  format: yaml
  label: groundmail-dev Smtp Credentials API
  slug: groundmail-dev-smtpcredentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-smtpcredentials-api-openapi.yml
- filename: groundmail-dev-suppressions-api-openapi.yml
  format: yaml
  label: groundmail-dev Suppressions API
  slug: groundmail-dev-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-suppressions-api-openapi.yml
- filename: groundmail-dev-templates-api-openapi.yml
  format: yaml
  label: groundmail-dev Templates API
  slug: groundmail-dev-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-templates-api-openapi.yml
- filename: groundmail-dev-tenants-api-openapi.yml
  format: yaml
  label: groundmail-dev Tenants API
  slug: groundmail-dev-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-tenants-api-openapi.yml
- filename: groundmail-dev-test-inbox-api-openapi.yml
  format: yaml
  label: groundmail-dev Test inbox API
  slug: groundmail-dev-test-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-test-inbox-api-openapi.yml
- filename: groundmail-dev-validation-api-openapi.yml
  format: yaml
  label: groundmail-dev Validation API
  slug: groundmail-dev-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-validation-api-openapi.yml
- filename: groundmail-dev-webhooks-api-openapi.yml
  format: yaml
  label: groundmail-dev Webhooks API
  slug: groundmail-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-webhooks-api-openapi.yml
- filename: groundmail-dev-api-keys-api-openapi.yml
  format: yaml
  label: groundmail-dev API Keys API
  slug: groundmail-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-api-keys-api-openapi.yml
auth_types: []
description: Authentication methods documented for Groundmail API
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Groundmail Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: groundmail-dev declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: groundmail-dev
provider_slug: groundmail-dev
scheme_count: 4
schemes:
- evidence: 'Groundmail authenticates API requests with a Bearer credential: an API key ( gm_… ) for servers and CI, a short-lived OAuth access token ( gm_oat_… ) for the CLI and agents, or, from Azure, a managed identity token with no key at all.'
  header: Authorization
  how_to_obtain: Create in the dashboard → API Keys → Create and copy the secret (shown once).
  location: header
  name: API key
  type: http-bearer
- evidence: 'Workloads on Azure (Container Apps, App Service, Functions, AKS workload identity, VMs) can authenticate with their managed identity instead of a key: the app gets a short-lived Microsoft Entra access token from Azure and sends it as Authorization: Bearer <token> .'
  header: Authorization
  how_to_obtain: Configure a managed identity in Azure, then use DefaultAzureCredential with the scope https://api.groundmail.dev/.default to acquire a token.
  location: header
  name: Azure managed identity token
  type: http-bearer
- evidence: 'Other tools can use the same flow, the OAuth 2.0 Device Authorization Grant (RFC 8628):'
  how_to_obtain: POST https://api.groundmail.dev/oauth/device_authorization with client_id and scope, then poll https://api.groundmail.dev/oauth/token.
  name: OAuth Device Authorization Grant
  scopes:
  - openid
  - email
  - emails:send
  - domains:read
  - etc.
  token_url: https://api.groundmail.dev/oauth/token
  type: oauth2
- authorize_url: https://app.groundmail.dev/.well-known/oauth-authorization-server
  evidence: 'The hosted MCP server signs clients in the same way, with the authorization code flow (PKCE): the person approving picks the scopes the client gets, and the connection appears under Settings → CLIs & agents with its scopes, where it can be revoked.'
  how_to_obtain: Run groundmail login which opens the browser for the authorization code flow.
  name: Authorization Code Flow (PKCE) for MCP clients
  token_url: https://api.groundmail.dev/oauth/token
  type: oauth2
slug: groundmail-dev-authentication
source_filename: groundmail-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.groundmail.dev/authentication
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.groundmail.dev/authentication\nsources:\n- https://docs.groundmail.dev/authentication\n- https://docs.groundmail.dev/authentication/azure-managed-identity\n- https://docs.groundmail.dev/api-keys\n- https://docs.groundmail.dev/guides/better-auth\ndescription: Authentication methods documented for Groundmail API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Groundmail authenticates API requests with a Bearer credential: an API key ( gm_… ) for servers and CI, a short-lived OAuth access\n    token ( gm_oat_… ) for the CLI and agents, or, from Azure, a managed identity token with no key at all.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create in the dashboard → API Keys → Create and copy the secret (shown once).\n- type: http-bearer\n  name: Azure managed identity token\n  evidence: 'Workloads on Azure (Container Apps, App Service,\
  \ Functions, AKS workload identity, VMs) can authenticate with their managed identity\n    instead of a key: the app gets a short-lived Microsoft Entra access token from Azure and sends it as Authorization: Bearer <token> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Configure a managed identity in Azure, then use DefaultAzureCredential with the scope https://api.groundmail.dev/.default to\n    acquire a token.\n- type: oauth2\n  name: OAuth Device Authorization Grant\n  evidence: 'Other tools can use the same flow, the OAuth 2.0 Device Authorization Grant (RFC 8628):'\n  token_url: https://api.groundmail.dev/oauth/token\n  scopes:\n  - openid\n  - email\n  - emails:send\n  - domains:read\n  - etc.\n  how_to_obtain: POST https://api.groundmail.dev/oauth/device_authorization with client_id and scope, then poll https://api.groundmail.dev/oauth/token.\n- type: oauth2\n  name: Authorization Code Flow (PKCE) for MCP clients\n  evidence: 'The hosted MCP server signs clients\
  \ in the same way, with the authorization code flow (PKCE): the person approving picks the scopes\n    the client gets, and the connection appears under Settings → CLIs & agents with its scopes, where it can be revoked.'\n  token_url: https://api.groundmail.dev/oauth/token\n  authorize_url: https://app.groundmail.dev/.well-known/oauth-authorization-server\n  how_to_obtain: Run groundmail login which opens the browser for the authorization code flow.\ndocs: https://docs.groundmail.dev/authentication\n"
source_yaml_url: https://artifacts.apis.io/groundmail-dev/authentication/groundmail-dev-authentication.yml
summary_line: 4 schemes
tags:
- Email
- API
- Transactional
- SMTP
- Developer
---
