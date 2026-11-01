---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sendmux-ai-billing-api-openapi.yml
  format: yaml
  label: sendmux-ai Billing API
  slug: sendmux-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-billing-api-openapi.yml
- filename: sendmux-ai-connection-api-openapi.yml
  format: yaml
  label: sendmux-ai Connection API
  slug: sendmux-ai-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-connection-api-openapi.yml
- filename: sendmux-ai-domain-filters-api-openapi.yml
  format: yaml
  label: sendmux-ai Domain Filters API
  slug: sendmux-ai-domain-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-domain-filters-api-openapi.yml
- filename: sendmux-ai-domains-api-openapi.yml
  format: yaml
  label: sendmux-ai Domains API
  slug: sendmux-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-domains-api-openapi.yml
- filename: sendmux-ai-emails-api-openapi.yml
  format: yaml
  label: sendmux-ai Emails API
  slug: sendmux-ai-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-emails-api-openapi.yml
- filename: sendmux-ai-inboxes-api-openapi.yml
  format: yaml
  label: sendmux-ai Inboxes API
  slug: sendmux-ai-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-inboxes-api-openapi.yml
- filename: sendmux-ai-mailbox-api-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailbox API
  slug: sendmux-ai-mailbox-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailbox-api-api-openapi.yml
- filename: sendmux-ai-mailbox-filters-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailbox Filters API
  slug: sendmux-ai-mailbox-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailbox-filters-api-openapi.yml
- filename: sendmux-ai-mailboxes-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailboxes API
  slug: sendmux-ai-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailboxes-api-openapi.yml
- filename: sendmux-ai-sending-accounts-api-openapi.yml
  format: yaml
  label: sendmux-ai Sending accounts API
  slug: sendmux-ai-sending-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-sending-accounts-api-openapi.yml
- filename: sendmux-ai-webhooks-api-openapi.yml
  format: yaml
  label: sendmux-ai Webhooks API
  slug: sendmux-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for Sendmux APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sendmux Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: sendmux-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: sendmux-ai
provider_slug: sendmux-ai
scheme_count: 2
schemes:
- authorize_url: https://app.sendmux.ai/oauth/authorize
  evidence: Configure scoped OAuth access to the Sending, Mailbox, and Management APIs.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Register a client via POST https://app.sendmux.ai/oauth/register, then perform the authorisation request and exchange the code at the token endpoint.
  name: Sendmux OAuth
  scopes:
  - email.send
  - mailbox.read
  - provider.read
  - webhook.read
  type: oauth2
- evidence: Authorization string header required Sendmux API key. Use a root API key for Management API routes, or a mailbox credential for Mailbox API routes.
  header: Authorization
  how_to_obtain: Create a manual API key in the Sendmux dashboard under API Keys, or generate a mailbox API key via the Create a mailbox API key endpoint.
  name: API Key / Mailbox Credential
  type: http-bearer
slug: sendmux-ai-authentication
source_filename: sendmux-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://sendmux.ai/docs/developer-tools/oauth
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sendmux.ai/docs/developer-tools/oauth\nsources:\n- https://sendmux.ai/docs/developer-tools/oauth\n- https://sendmux.ai/docs/api/mailboxes/create-a-mailbox-api-key\n- https://sendmux.ai/docs/api/mailboxes/revoke-a-mailbox-api-key\n- https://sendmux.ai/docs/account/api-keys\ndescription: Authentication methods for Sendmux APIs\nschemes:\n- type: oauth2\n  name: Sendmux OAuth\n  evidence: Configure scoped OAuth access to the Sending, Mailbox, and Management APIs.\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://app.sendmux.ai/oauth/authorize\n  scopes:\n  - email.send\n  - mailbox.read\n  - provider.read\n  - webhook.read\n  how_to_obtain: Register a client via POST https://app.sendmux.ai/oauth/register, then perform the authorisation request and exchange the code\n    at the token endpoint.\n- type: http-bearer\n  name: API Key / Mailbox Credential\n\
  \  evidence: Authorization string header required Sendmux API key. Use a root API key for Management API routes, or a mailbox credential for Mailbox\n    API routes.\n  header: Authorization\n  how_to_obtain: Create a manual API key in the Sendmux dashboard under API Keys, or generate a mailbox API key via the Create a mailbox API key\n    endpoint.\ndocs: https://sendmux.ai/docs/developer-tools/oauth\n"
source_yaml_url: https://artifacts.apis.io/sendmux-ai/authentication/sendmux-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Email
- AI
- Agents
- Integration
---
