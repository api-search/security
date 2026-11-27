---
anonymous_access: true
api_key_in: []
api_specs:
- filename: capxule-ai-account-api-openapi.yml
  format: yaml
  label: Capxule Account API
  slug: capxule-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capxule-ai/openapi/capxule-ai-account-api-openapi.yml
- filename: capxule-ai-catalog-api-openapi.yml
  format: yaml
  label: Capxule Catalog API
  slug: capxule-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capxule-ai/openapi/capxule-ai-catalog-api-openapi.yml
- filename: capxule-ai-plan-api-openapi.yml
  format: yaml
  label: Capxule Plan API
  slug: capxule-ai-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capxule-ai/openapi/capxule-ai-plan-api-openapi.yml
auth_types:
- http
- oauth2
- apiKey
- none
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Capxule Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capxule secures its APIs with http, oauth2, apiKey, and none across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Capxule
provider_slug: capxule-ai
scheme_count: 6
schemes:
- description: oat_ access token with the journey scope family (from connector OAuth or the device grant).
  name: oauth
  scheme: bearer
  sources:
  - openapi/capxule-ai-openapi.yml
  type: http
- description: Connector OAuth on https://capxule.ai/mcp; authorization server https://app.capxule.com; protected-resource metadata at https://capxule.ai/.well-known/oauth-protected-resource (RFC 9728). The human signs in on capxule.com and the agent becomes a `delegated` principal.
  name: connector-oauth
  revocation: RFC 7009 revoke, also the `disconnect` tool
  sources:
  - https://capxule.ai/identity
  token_lifetimes: oat_ access (30 days) and ort_ refresh (90 days, single use, rotated; reuse revokes the whole family and emails the human)
  type: oauth2
- description: RFC 8628 device grant for CLI and headless agents. device_authorization_endpoint https://app.capxule.com/api/oauth/device; token endpoint https://app.capxule.com/api/oauth/token; verification_uri https://capxule.com/device. Device code 15 minutes, poll every 5 s.
  flow: urn:ietf:params:oauth:grant-type:device_code
  name: device-grant
  sources:
  - https://capxule.ai/protocols
  type: oauth2
- description: Guest (`open`) principal on https://capxule.ai/mcp/open keyed on a stable `_meta.subject` (or the Mcp-Session-Id issued on initialize); no credential. REST twins carry it as the X-Capxule-Subject header.
  name: open-subject
  sources:
  - https://capxule.ai/identity
  type: none
- description: '`machine` principal: a verified Web Bot Auth signature (RFC 9421; Signature-Agent directory, Ed25519, keyid = JWK thumbprint). Covered components must include @authority and signature-agent; created and expires required, 60 s skew, lifetime at most 24 h. An unverified signature is `anonymous`.'
  name: web-bot-auth
  sources:
  - https://capxule.ai/protocols
  type: http-message-signature
- description: Studio MCP connector (https://capxule.ai/mcp/studio) only. The creator makes a key on https://app.capxule.com/studio; sent as ?key=<studio key>, x-api-key, or Authorization Bearer.
  name: studio-key
  sources:
  - https://capxule.ai/llms.txt
  type: apiKey
slug: capxule-ai-authentication
source_filename: capxule-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://capxule.ai/identity\ndocs: https://capxule.ai/identity\nsee_also:\n- https://capxule.ai/protocols\n- https://capxule.ai/principals\nsummary:\n  types:\n  - http\n  - oauth2\n  - apiKey\n  - none\nschemes:\n- name: oauth\n  type: http\n  scheme: bearer\n  description: oat_ access token with the journey scope family (from connector OAuth or the device grant).\n  sources:\n  - openapi/capxule-ai-openapi.yml\n- name: connector-oauth\n  type: oauth2\n  description: Connector OAuth on https://capxule.ai/mcp; authorization server https://app.capxule.com; protected-resource metadata at https://capxule.ai/.well-known/oauth-protected-resource (RFC 9728). The human signs in on capxule.com and the agent becomes a `delegated` principal.\n  token_lifetimes: \"oat_ access (30 days) and ort_ refresh (90 days, single use, rotated; reuse revokes the whole family and emails the human)\"\n  revocation: RFC 7009 revoke, also the `disconnect`\
  \ tool\n  sources:\n  - https://capxule.ai/identity\n- name: device-grant\n  type: oauth2\n  flow: urn:ietf:params:oauth:grant-type:device_code\n  description: RFC 8628 device grant for CLI and headless agents. device_authorization_endpoint https://app.capxule.com/api/oauth/device; token endpoint https://app.capxule.com/api/oauth/token; verification_uri https://capxule.com/device. Device code 15 minutes, poll every 5 s.\n  sources:\n  - https://capxule.ai/protocols\n- name: open-subject\n  type: none\n  description: Guest (`open`) principal on https://capxule.ai/mcp/open keyed on a stable `_meta.subject` (or the Mcp-Session-Id issued on initialize); no credential. REST twins carry it as the X-Capxule-Subject header.\n  sources:\n  - https://capxule.ai/identity\n- name: web-bot-auth\n  type: http-message-signature\n  description: \"`machine` principal: a verified Web Bot Auth signature (RFC 9421; Signature-Agent directory, Ed25519, keyid = JWK thumbprint). Covered components must include\
  \ @authority and signature-agent; created and expires required, 60 s skew, lifetime at most 24 h. An unverified signature is `anonymous`.\"\n  sources:\n  - https://capxule.ai/protocols\n- name: studio-key\n  type: apiKey\n  description: Studio MCP connector (https://capxule.ai/mcp/studio) only. The creator makes a key on https://app.capxule.com/studio; sent as ?key=<studio key>, x-api-key, or Authorization Bearer.\n  sources:\n  - https://capxule.ai/llms.txt\n"
source_yaml_url: https://artifacts.apis.io/capxule-ai/authentication/capxule-ai-authentication.yml
summary_line: http/oauth2/apiKey/none · 6 schemes
tags:
- Company
- Context Marketplace
- Artificial Intelligence
- AI Agents
- MCP
- Education
- Test Preparation
- Knowledge
---
