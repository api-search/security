---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Segmetrics Authentication
name_suffix: Authentication
oauth_flows:
- unspecified
overview: SegMetrics secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the unspecified flow(s).
provider_name: SegMetrics
provider_slug: segmetrics
scheme_count: 3
schemes:
- applies_to:
  - Import API (https://import.segmetrics.io/api/v1/{account_id}/{integration_id}/)
  - Reporting API (https://api.segmetrics.io/)
  - Contact API (https://api.segmetrics.io/{account_id}/contact/{id_or_email})
  format: raw-key
  format_note: 'The key is sent as the bare value of the Authorization header — no "Bearer" or "Token" prefix is documented. Example published by SegMetrics: `-H ''Authorization: YOUR_API_KEY''`.'
  in: header
  key_issuance: Account ID and API Key are both found on the SegMetrics Account page (https://app.segmetrics.io/a/account/edit). No self-service key rotation, scoping, or expiry is documented.
  name: ApiKeyAuth
  parameter_name: Authorization
  sources:
  - https://developers.segmetrics.io/#authentication
  type: apiKey
- applies_to:
  - MCP Server (https://app.segmetrics.io/mcp/{ACCOUNT_ID})
  flows: []
  flows_note: SegMetrics documents that connecting the MCP server prompts an OAuth authorization against the SegMetrics account, but publishes no authorization/token endpoints, no scope reference, and no /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource metadata. The flow is therefore recorded as present-but-undocumented rather than guessed.
  name: OAuth
  sources:
  - https://docs.segmetrics.io/article/672-mcp-server
  type: oauth2
- applies_to:
  - JS API (browser tracking snippet)
  name: JavaScriptSnippet
  note: The client-side JS API is authorized by the account-scoped tracking snippet installed on the customer's own pages, not by an API key. It identifies visitors; it does not read data.
  sources:
  - https://developers.segmetrics.io/#js_getting_started
  type: other
slug: segmetrics-authentication
source_filename: segmetrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developers.segmetrics.io/#authentication\ndocs: https://developers.segmetrics.io/#authentication\nnote: >-\n  SegMetrics publishes no OpenAPI, so this profile is transcribed from the published API\n  reference rather than derived from securitySchemes. Two distinct auth models are in use: a\n  static API key on the REST surfaces, and OAuth on the MCP server.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_names: [Authorization]\n  oauth2_flows: [unspecified]\n  tenancy: >-\n    Account ID is a PATH segment on every REST call, so the API key alone does not select the\n    tenant — the caller must know both the Account ID and, on the Import API, the Integration ID.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: raw-key\n  format_note: >-\n    The key is sent as the bare value of the Authorization header — no \"Bearer\" or \"Token\"\n    prefix\
  \ is documented. Example published by SegMetrics: `-H 'Authorization: YOUR_API_KEY'`.\n  applies_to:\n  - Import API (https://import.segmetrics.io/api/v1/{account_id}/{integration_id}/)\n  - Reporting API (https://api.segmetrics.io/)\n  - Contact API (https://api.segmetrics.io/{account_id}/contact/{id_or_email})\n  key_issuance: >-\n    Account ID and API Key are both found on the SegMetrics Account page\n    (https://app.segmetrics.io/a/account/edit). No self-service key rotation, scoping, or\n    expiry is documented.\n  sources: ['https://developers.segmetrics.io/#authentication']\n- name: OAuth\n  type: oauth2\n  applies_to:\n  - MCP Server (https://app.segmetrics.io/mcp/{ACCOUNT_ID})\n  flows: []\n  flows_note: >-\n    SegMetrics documents that connecting the MCP server prompts an OAuth authorization against\n    the SegMetrics account, but publishes no authorization/token endpoints, no scope reference,\n    and no /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource\n\
  \    metadata. The flow is therefore recorded as present-but-undocumented rather than guessed.\n  sources: ['https://docs.segmetrics.io/article/672-mcp-server']\n- name: JavaScriptSnippet\n  type: other\n  applies_to:\n  - JS API (browser tracking snippet)\n  note: >-\n    The client-side JS API is authorized by the account-scoped tracking snippet installed on\n    the customer's own pages, not by an API key. It identifies visitors; it does not read data.\n  sources: ['https://developers.segmetrics.io/#js_getting_started']\ngaps:\n- No documented key rotation, expiry, or scoping on the REST API key.\n- No OAuth scope reference published for the MCP surface.\n- No RFC 8414 / RFC 9728 discovery metadata on any host (see well-known/segmetrics-well-known.yml).\nx-evidence:\n  fetched: '2026-08-12'\n  sources:\n  - {url: 'https://developers.segmetrics.io/', status: 200}\n  - {url: 'https://docs.segmetrics.io/article/672-mcp-server', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segmetrics/refs/heads/main/authentication/segmetrics-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Marketing
- Analytics
- Attribution
- Marketing Analytics
- Reporting
- Business Intelligence
- Advertising
- Software-as-a-Service
- MCP
---
