---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Plain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plain secures its APIs with apiKey, oauth2, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Plain
provider_slug: plain
scheme_count: 4
schemes:
- format: Bearer plainApiKey_xxx
  header: Authorization
  in: header
  name: apiKey
  note: API keys belong to Machine Users and carry fine-grained permissions selected at creation. A Machine User can hold multiple keys for rotation. Keys are shown once and cannot be retrieved again.
  type: apiKey
- name: permissions
  note: Calls are authorized against per-key permissions (e.g. indexedDocument:create, thread:reply). Insufficient permissions return an error naming the permission required.
  type: rbac
- name: oauth2
  note: OAuth is used by the hosted MCP server (mcp.plain.com/mcp); an agent authenticates as an existing Plain user and inherits that user's permissions.
  type: oauth2
- docs: https://www.plain.com/docs/mtls
  name: mutualTLS
  note: mTLS is supported for webhook delivery and customer-card requests.
  type: mutualTLS
slug: plain-authentication
source_filename: plain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.plain.com/docs/graphql/authentication.md\ndocs: https://www.plain.com/docs/graphql/authentication\nsummary:\n  types: [apiKey, oauth2, mutualTLS]\n  api_key_in: [header]\n  api_key_prefix: plainApiKey_\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    header: Authorization\n    format: \"Bearer plainApiKey_xxx\"\n    note: >-\n      API keys belong to Machine Users and carry fine-grained permissions\n      selected at creation. A Machine User can hold multiple keys for rotation.\n      Keys are shown once and cannot be retrieved again.\n  - name: permissions\n    type: rbac\n    note: >-\n      Calls are authorized against per-key permissions (e.g.\n      indexedDocument:create, thread:reply). Insufficient permissions return an\n      error naming the permission required.\n  - name: oauth2\n    type: oauth2\n    note: >-\n      OAuth is used by the hosted MCP server (mcp.plain.com/mcp); an agent\n\
  \      authenticates as an existing Plain user and inherits that user's\n      permissions.\n  - name: mutualTLS\n    type: mutualTLS\n    docs: https://www.plain.com/docs/mtls\n    note: mTLS is supported for webhook delivery and customer-card requests.\nwebhook_verification:\n  request_signing:\n    docs: https://www.plain.com/docs/request-signing\n    header: Plain-Request-Signature\n    algorithm: HMAC-SHA256\n    encoding: hex\n    note: >-\n      Workspace-global HMAC secret (Settings -> Request signing). The signature\n      is the HMAC-SHA256 of the raw request body, hex-encoded.\n  basic_auth: true\n  mtls: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plain/refs/heads/main/authentication/plain-authentication.yml
summary_line: apiKey/oauth2/mutualTLS · 4 schemes
tags:
- Company
- Customer Support
- Customer Service
- Help Desk
- Support
- SaaS
- GraphQL
- Webhooks
- MCP
- Developer Tools
---
