---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: ClutchCall Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClutchCall declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: ClutchCall
provider_slug: clutchcall-dev
scheme_count: 6
schemes:
- description: Long-lived key scoped to one org and a set of capabilities; authenticates every control-plane call over HTTPS. Shown once at creation, only the hash is stored. Scopes fixed at creation.
  docs: https://docs.clutchcall.dev/admin/api-keys
  env_var: CLUTCHCALL_API_KEY
  example_prefix: tqs_live_
  name: control-plane API key
  type: apiKey
- bearerFormat: JWT (EdDSA)
  description: Short-lived signed JWT minted from an API key, carrying namespace claims (ns); presented during the MoQT handshake and checked by the relay namespace_auth hook. Typically 1h for client tokens.
  docs: https://docs.clutchcall.dev/concepts/authentication
  name: relay token
  scheme: bearer
  type: http
- description: Short-lived token minted server-side (e.g. voice.audioBridge.mintBrowserToken) so no API key ships to the browser.
  docs: https://docs.clutchcall.dev/concepts/authentication
  name: browser token
  scheme: bearer
  type: http
- description: Platform MCP at https://portal.clutchcall.dev/mcp accepts a console session JWT or an MCP access key (prefix mpk_) sent as Bearer in Authorization; scopes mcp:<domain>:<action>. Publishes OAuth 2.0 Protected Resource Metadata naming authorization server https://portal.clutchcall.dev/auth/v1.
  docs: https://docs.clutchcall.dev/platform/mcp
  name: MCP access key / OAuth
  prm: https://portal.clutchcall.dev/.well-known/oauth-protected-resource
  type: oauth2
- bearerFormat: RS256 JWT
  description: Original ClutchCallClient root import signed an RS256 JWT from a service-account JSON (CLUTCHCALL_CREDENTIALS) on the QUIC handshake; still works for backwards compatibility.
  docs: https://docs.clutchcall.dev/concepts/authentication
  name: legacy service-account JWT
  scheme: bearer
  type: http
- description: Inference HTTP surface authenticates with bearer API keys.
  docs: https://docs.clutchcall.dev/modalities/inference/openai-compatible-api
  name: OpenAI-compatible inference bearer key
  scheme: bearer
  type: http
slug: clutchcall-dev-authentication
source_filename: clutchcall-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.clutchcall.dev/concepts/authentication\ndocs: https://docs.clutchcall.dev/concepts/authentication\nschemes:\n- name: control-plane API key\n  type: apiKey\n  description: Long-lived key scoped to one org and a set of capabilities; authenticates every control-plane call over HTTPS. Shown once at creation, only the hash is stored. Scopes fixed at creation.\n  example_prefix: tqs_live_\n  env_var: CLUTCHCALL_API_KEY\n  docs: https://docs.clutchcall.dev/admin/api-keys\n- name: relay token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT (EdDSA)\n  description: Short-lived signed JWT minted from an API key, carrying namespace claims (ns); presented during the MoQT handshake and checked by the relay namespace_auth hook. Typically 1h for client tokens.\n  docs: https://docs.clutchcall.dev/concepts/authentication\n- name: browser token\n  type: http\n  scheme: bearer\n  description: Short-lived token minted server-side\
  \ (e.g. voice.audioBridge.mintBrowserToken) so no API key ships to the browser.\n  docs: https://docs.clutchcall.dev/concepts/authentication\n- name: MCP access key / OAuth\n  type: oauth2\n  description: Platform MCP at https://portal.clutchcall.dev/mcp accepts a console session JWT or an MCP access key (prefix mpk_) sent as Bearer in Authorization; scopes mcp:<domain>:<action>. Publishes\n    OAuth 2.0 Protected Resource Metadata naming authorization server https://portal.clutchcall.dev/auth/v1.\n  prm: https://portal.clutchcall.dev/.well-known/oauth-protected-resource\n  docs: https://docs.clutchcall.dev/platform/mcp\n- name: legacy service-account JWT\n  type: http\n  scheme: bearer\n  bearerFormat: RS256 JWT\n  description: Original ClutchCallClient root import signed an RS256 JWT from a service-account JSON (CLUTCHCALL_CREDENTIALS) on the QUIC handshake; still works for backwards compatibility.\n  docs: https://docs.clutchcall.dev/concepts/authentication\n- name: OpenAI-compatible\
  \ inference bearer key\n  type: http\n  scheme: bearer\n  description: Inference HTTP surface authenticates with bearer API keys.\n  docs: https://docs.clutchcall.dev/modalities/inference/openai-compatible-api\nrelated_docs:\n- https://docs.clutchcall.dev/admin/api-keys\n- https://docs.clutchcall.dev/concepts/credentials\n- https://docs.clutchcall.dev/platform/mcp\n"
source_yaml_url: https://artifacts.apis.io/clutchcall-dev/authentication/clutchcall-dev-authentication.yml
summary_line: 6 schemes
tags:
- Company
- Voice AI
- Real-Time Communication
- QUIC
- Telephony
- SIP
- Live Streaming
- Robotics
- Inference
- WebTransport
---
