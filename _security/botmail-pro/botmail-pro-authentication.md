---
anonymous_access: false
api_key_in: []
api_specs:
- filename: botmail-pro-account-api-openapi.yml
  format: yaml
  label: Botmail Account API
  slug: botmail-pro-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-account-api-openapi.yml
- filename: botmail-pro-billing-api-openapi.yml
  format: yaml
  label: Botmail Billing API
  slug: botmail-pro-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-billing-api-openapi.yml
- filename: botmail-pro-claim-api-openapi.yml
  format: yaml
  label: Botmail Claim API
  slug: botmail-pro-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-claim-api-openapi.yml
- filename: botmail-pro-events-api-openapi.yml
  format: yaml
  label: Botmail Events API
  slug: botmail-pro-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-events-api-openapi.yml
- filename: botmail-pro-keys-api-openapi.yml
  format: yaml
  label: Botmail Keys API
  slug: botmail-pro-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-keys-api-openapi.yml
- filename: botmail-pro-mail-api-openapi.yml
  format: yaml
  label: Botmail Mail API
  slug: botmail-pro-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-mail-api-openapi.yml
- filename: botmail-pro-mailboxes-api-openapi.yml
  format: yaml
  label: Botmail Mailboxes API
  slug: botmail-pro-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-mailboxes-api-openapi.yml
- filename: botmail-pro-meta-api-openapi.yml
  format: yaml
  label: Botmail Meta API
  slug: botmail-pro-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-meta-api-openapi.yml
- filename: botmail-pro-send-api-openapi.yml
  format: yaml
  label: Botmail Send API
  slug: botmail-pro-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-send-api-openapi.yml
- filename: botmail-pro-webhooks-api-openapi.yml
  format: yaml
  label: Botmail Webhooks API
  slug: botmail-pro-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-webhooks-api-openapi.yml
auth_types: []
description: Botmail authenticates API requests using a bearer token supplied in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Botmail Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Botmail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Botmail
provider_slug: botmail-pro
scheme_count: 1
schemes:
- evidence: 'curl -s https://botmail.pro/v1/webhooks \ -H "Authorization: Bearer $BOTMAIL_KEY" \ -H ''Content-Type: application/json'' \ -d ''{"url": "https://agent.example.com/botmail", "events": ["message.received"]}'''
  header: Authorization
  how_to_obtain: A key is returned when you claim an address with the Botmail CLI (e.g., `npx botmail claim ada --human you@example.com`).
  location: header
  name: Botmail API Key
  type: http-bearer
slug: botmail-pro-authentication
source_filename: botmail-pro-authentication.yml
source_heading: Authentication Profile
source_url: https://botmail.pro/compare/nylas
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://botmail.pro/compare/nylas\nsources:\n- https://botmail.pro/compare/nylas\n- https://botmail.pro/guides/email-webhooks-for-ai-agents\ndescription: Botmail authenticates API requests using a bearer token supplied in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Botmail API Key\n  evidence: 'curl -s https://botmail.pro/v1/webhooks \\ -H \"Authorization: Bearer $BOTMAIL_KEY\" \\ -H ''Content-Type: application/json'' \\ -d ''{\"url\":\n    \"https://agent.example.com/botmail\", \"events\": [\"message.received\"]}'''\n  location: header\n  header: Authorization\n  how_to_obtain: A key is returned when you claim an address with the Botmail CLI (e.g., `npx botmail claim ada --human you@example.com`).\nnote: No OAuth2 flows, API keys, or other authentication methods are documented on the referenced pages.\ndocs: https://botmail.pro/compare/nylas\n"
source_yaml_url: https://artifacts.apis.io/botmail-pro/authentication/botmail-pro-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Email
- Messaging
- Automation
- Botmail
---
