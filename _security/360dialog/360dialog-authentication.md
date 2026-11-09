---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 360dialog-openapi-generated.yml
  format: yaml
  label: 360dialog API
  slug: 360dialog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/360dialog/openapi/_ae-authored/360dialog-openapi-generated.yml
auth_types: []
description: Authentication methods for 360dialog Business Agent API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: 360Dialog Authentication
name_suffix: Authentication
oauth_flows: []
overview: 360dialog declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: 360dialog
provider_slug: 360dialog
scheme_count: 1
schemes:
- evidence: API Key for Messaging API authentication. Send your API key in the D360-API-KEY header.
  header: D360-API-KEY
  how_to_obtain: Provided by 360dialog when you create a Business Account
  location: header
  name: D360-API-KEY
  type: apiKey
slug: 360dialog-authentication
source_filename: 360dialog-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.360dialog.com/docs/mba/api-ref/knowledge-connectors/upsert-api-key-credentials-for-a-connector.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.360dialog.com/docs/mba/api-ref/knowledge-connectors/upsert-api-key-credentials-for-a-connector.md\nsources:\n- https://docs.360dialog.com/docs/mba/api-ref/knowledge-connectors/upsert-api-key-credentials-for-a-connector.md\n- https://docs.360dialog.com/docs/mba/api-ref/knowledge-connectors/upsert-oauth-2-0-credentials-for-a-connector.md\n- https://docs.360dialog.com/docs/resources/authentication-messages.md\n- https://docs.360dialog.com/docs/resources/authentication-messages/autofill-button-authentication-templates.md\ndescription: Authentication methods for 360dialog Business Agent API\nschemes:\n- type: apiKey\n  name: D360-API-KEY\n  evidence: API Key for Messaging API authentication. Send your API key in the D360-API-KEY header.\n  location: header\n  header: D360-API-KEY\n  how_to_obtain: Provided by 360dialog when you create a Business Account\nnote: OAuth client‑credentials\
  \ are described only as request payload fields; no token or authorize URLs are published, so no OAuth scheme is listed.\ndocs: https://docs.360dialog.com/docs/mba/api-ref/knowledge-connectors/upsert-api-key-credentials-for-a-connector.md\n"
source_yaml_url: https://artifacts.apis.io/360dialog/authentication/360dialog-authentication.yml
summary_line: 1 scheme
tags:
- Company
- WhatsApp
- Messaging
- Business
---
