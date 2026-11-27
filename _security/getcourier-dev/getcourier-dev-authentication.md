---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getcourier-dev-accounts-api-openapi.yml
  format: yaml
  label: Nuvidian AI, LLC Accounts API
  slug: getcourier-dev-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcourier-dev/openapi/getcourier-dev-accounts-api-openapi.yml
- filename: getcourier-dev-deposits-api-openapi.yml
  format: yaml
  label: Nuvidian AI, LLC Deposits API
  slug: getcourier-dev-deposits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcourier-dev/openapi/getcourier-dev-deposits-api-openapi.yml
- filename: getcourier-dev-inboxes-api-openapi.yml
  format: yaml
  label: Nuvidian AI, LLC Inboxes API
  slug: getcourier-dev-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcourier-dev/openapi/getcourier-dev-inboxes-api-openapi.yml
- filename: getcourier-dev-meta-api-openapi.yml
  format: yaml
  label: Nuvidian AI, LLC Meta API
  slug: getcourier-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcourier-dev/openapi/getcourier-dev-meta-api-openapi.yml
- filename: getcourier-dev-sandbox-api-openapi.yml
  format: yaml
  label: Nuvidian AI, LLC Sandbox API
  slug: getcourier-dev-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcourier-dev/openapi/getcourier-dev-sandbox-api-openapi.yml
auth_types: []
description: GetCourier uses bearer tokens for reading inboxes and for MCP calls; no API key or signup is required for creating an inbox.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nuvidian AI, LLC Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuvidian AI, LLC declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nuvidian AI, LLC
provider_slug: getcourier-dev
scheme_count: 1
schemes:
- evidence: 'The read endpoints take the same bearer token. Use them when the agent wants to inspect a mailbox rather than wait on one message: curl -s -H "Authorization: Bearer $READ_TOKEN" "https://getcourier.dev/v1/sandbox/inboxes/$ALIAS/messages"'
  header: Authorization
  how_to_obtain: A read_token is returned in the JSON response when creating an inbox via an unauthenticated POST to https://getcourier.dev/alias.
  location: header
  name: Bearer token
  type: http-bearer
slug: getcourier-dev-authentication
source_filename: getcourier-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://getcourier.dev/email-inbox-without-signup
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getcourier.dev/email-inbox-without-signup\nsources:\n- https://getcourier.dev/email-inbox-without-signup\n- https://getcourier.dev/guides/mcp/\ndescription: GetCourier uses bearer tokens for reading inboxes and for MCP calls; no API key or signup is required for creating an inbox.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'The read endpoints take the same bearer token. Use them when the agent wants to inspect a mailbox rather than wait on one message:\n    curl -s -H \"Authorization: Bearer $READ_TOKEN\" \"https://getcourier.dev/v1/sandbox/inboxes/$ALIAS/messages\"'\n  location: header\n  header: Authorization\n  how_to_obtain: A read_token is returned in the JSON response when creating an inbox via an unauthenticated POST to https://getcourier.dev/alias.\nnote: No other authentication methods (apiKey, oauth2, http-basic, jwt, hmac, mtls, other) are\
  \ documented.\ndocs: https://getcourier.dev/email-inbox-without-signup\n"
source_yaml_url: https://artifacts.apis.io/getcourier-dev/authentication/getcourier-dev-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Artificial Intelligence
- Agents
- Automation
- Services
---
