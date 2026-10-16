---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emailconnect-api-v1-emails-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI API v1 - Emails API
  slug: emailconnect-api-v1-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-api-v1-emails-api-openapi.yml
- filename: emailconnect-api-v1-logs-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI API v1 - Logs API
  slug: emailconnect-api-v1-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-api-v1-logs-api-openapi.yml
- filename: emailconnect-api-v1-metrics-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI API v1 - Metrics API
  slug: emailconnect-api-v1-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-api-v1-metrics-api-openapi.yml
- filename: emailconnect-user-aliases-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI User Aliases API
  slug: emailconnect-user-aliases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-user-aliases-api-openapi.yml
- filename: emailconnect-user-domains-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI User Domains API
  slug: emailconnect-user-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-user-domains-api-openapi.yml
- filename: emailconnect-user-webhooks-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI User Webhooks API
  slug: emailconnect-user-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-user-webhooks-api-openapi.yml
- filename: emailconnect-webhook-alias-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI Webhook Alias API
  slug: emailconnect-webhook-alias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-webhook-alias-api-openapi.yml
auth_types: []
description: Authentication for EmailConnect API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Emailconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: EmailConnect by XADI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EmailConnect by XADI
provider_slug: emailconnect
scheme_count: 1
schemes:
- evidence: Authenticate every request with the X-API-KEY header.
  header: X-API-KEY
  how_to_obtain: Create API key in the dashboard via Settings > API Keys and click "Generate key".
  location: header
  name: X-API-KEY
  type: apiKey
slug: emailconnect-authentication
source_filename: emailconnect-authentication.yml
source_heading: Authentication Profile
source_url: https://emailconnect.eu/help/api-keys-integrations/
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://emailconnect.eu/help/api-keys-integrations/\nsources:\n- https://emailconnect.eu/help/api-keys-integrations/\n- https://emailconnect.eu/help/webhook-signing/\n- https://emailconnect.eu/help/getting-started/\n- https://emailconnect.eu/help/domain-setup/\ndescription: Authentication for EmailConnect API\nschemes:\n- type: apiKey\n  name: X-API-KEY\n  evidence: Authenticate every request with the X-API-KEY header.\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Create API key in the dashboard via Settings > API Keys and click \"Generate key\".\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, MTLS, or other authentication schemes are documented on the provided pages.\ndocs: https://emailconnect.eu/help/api-keys-integrations/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/authentication/emailconnect-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email
- Webhook
- EU
- Compliance
---
