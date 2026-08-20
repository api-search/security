---
api_key_in: []
auth_types: []
description: Kixie authenticates every documented API surface with a single, long-lived, account-scoped API key paired with a numeric Business ID. There is no OAuth 2.0 authorization server, no OpenID Connect discovery document, no scope model, no per-user credential and no token exchange. The key is issued once per Kixie account (not per user) and must be activated by Kixie Support before first use.
kind: authentication
layout: security
method: searched
name: Kixie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kixie declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Kixie
provider_slug: kixie
scheme_count: 4
schemes:
- applies_to:
  - Kixie Event API
  - Kixie Webhook Management API
  description: The account API key, passed as a query-string parameter on the request URL. Used by the Event API (POST https://apig.kixie.com/app/event?apikey=...) and the legacy queue endpoints.
  evidence: https://developer.kixie.com/make-a-call/
  id: kixie-api-key-query
  in: query
  name: apikey
  required: true
  type: apiKey
- applies_to:
  - Kixie Event API
  - Kixie Webhook Management API
  description: The same account API key, repeated inside the JSON request body. Kixie's PowerList API documentation states this explicitly — "Your API key is already in the endpoint URL, but must be in the API body as well" — so both placements are required together, not alternatives.
  evidence: https://support.kixie.com/hc/en-us/articles/19135310564635-PowerList-API
  id: kixie-api-key-body
  in: body
  name: apikey
  required: true
  type: apiKey
- applies_to:
  - Kixie Agent Status API
  description: The Agent Status API uses a camel-cased `apiKey` query parameter rather than the lower-cased `apikey` every other endpoint uses. This inconsistency is in Kixie's own documentation and is a real integration hazard, not a transcription error on our part.
  evidence: https://support.kixie.com/hc/en-us/articles/360020051474-Kixie-Agent-Status-API
  id: kixie-api-key-query-camel
  in: query
  name: apiKey
  required: true
  type: apiKey
- applies_to:
  - Kixie Event API
  - Kixie Webhook Management API
  description: The numeric Kixie Business ID that scopes the request to an account. Not a secret in the cryptographic sense, but required alongside the API key on every Event API and Webhook Management call; requests without it are not account-resolvable.
  evidence: https://support.kixie.com/hc/en-us/articles/7273987300635-Kixie-Authentication-Overview
  id: kixie-business-id
  in: body
  name: businessid
  required: true
  type: tenantIdentifier
slug: kixie-authentication
source_filename: kixie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://support.kixie.com/hc/en-us/articles/7273987300635-Kixie-Authentication-Overview\ndocs: https://support.kixie.com/hc/en-us/articles/7273987300635-Kixie-Authentication-Overview\n\nname: Kixie authentication profile\ndescription: >-\n  Kixie authenticates every documented API surface with a single, long-lived, account-scoped API\n  key paired with a numeric Business ID. There is no OAuth 2.0 authorization server, no OpenID\n  Connect discovery document, no scope model, no per-user credential and no token exchange. The\n  key is issued once per Kixie account (not per user) and must be activated by Kixie Support\n  before first use.\n\nderived_from: docs\nnote: >-\n  Derived from Kixie's published authentication overview and the request examples on\n  developer.kixie.com. Kixie publishes no OpenAPI, so there are no securitySchemes to parse —\n  this profile is read from the human documentation.\n\nschemes:\n- id: kixie-api-key-query\n\
  \  type: apiKey\n  in: query\n  name: apikey\n  description: >-\n    The account API key, passed as a query-string parameter on the request URL. Used by the Event\n    API (POST https://apig.kixie.com/app/event?apikey=...) and the legacy queue endpoints.\n  required: true\n  applies_to:\n  - Kixie Event API\n  - Kixie Webhook Management API\n  evidence: https://developer.kixie.com/make-a-call/\n\n- id: kixie-api-key-body\n  type: apiKey\n  in: body\n  name: apikey\n  description: >-\n    The same account API key, repeated inside the JSON request body. Kixie's PowerList API\n    documentation states this explicitly — \"Your API key is already in the endpoint URL, but must\n    be in the API body as well\" — so both placements are required together, not alternatives.\n  required: true\n  applies_to:\n  - Kixie Event API\n  - Kixie Webhook Management API\n  evidence: https://support.kixie.com/hc/en-us/articles/19135310564635-PowerList-API\n\n- id: kixie-api-key-query-camel\n  type: apiKey\n\
  \  in: query\n  name: apiKey\n  description: >-\n    The Agent Status API uses a camel-cased `apiKey` query parameter rather than the lower-cased\n    `apikey` every other endpoint uses. This inconsistency is in Kixie's own documentation and is\n    a real integration hazard, not a transcription error on our part.\n  required: true\n  applies_to:\n  - Kixie Agent Status API\n  evidence: https://support.kixie.com/hc/en-us/articles/360020051474-Kixie-Agent-Status-API\n\n- id: kixie-business-id\n  type: tenantIdentifier\n  in: body\n  name: businessid\n  description: >-\n    The numeric Kixie Business ID that scopes the request to an account. Not a secret in the\n    cryptographic sense, but required alongside the API key on every Event API and Webhook\n    Management call; requests without it are not account-resolvable.\n  required: true\n  applies_to:\n  - Kixie Event API\n  - Kixie Webhook Management API\n  evidence: https://support.kixie.com/hc/en-us/articles/7273987300635-Kixie-Authentication-Overview\n\
  \ncredential_issuance:\n  self_service: false\n  path: Kixie Dashboard > Manage > Account Settings > Integrations\n  requires_role: Admin\n  requires_activation: true\n  activation_note: >-\n    Kixie states the API key must be activated by Support before an integration will work —\n    \"you may need to contact Support via live chat in order for us to enable your API key.\"\n  plan_gate: >-\n    Kixie's PowerList API documentation requires \"a paid Kixie account with at least one\n    Professional tier agent\"; the Team SMS and Send to Queue articles state the Professional\n    Billing Tier or higher.\n\ngranularity:\n  scope: account\n  per_user_credentials: false\n  key_count_per_account: 1\n  note: >-\n    \"Each key and BID is specific to a Kixie account, not an individual user, and only one key\n    and BID are assigned to an account.\" One credential per tenant means no per-integration\n    revocation and no least-privilege split between an automation and a human operator.\n\ngaps:\n\
  - id: key-in-query-string\n  severity: high\n  finding: >-\n    The API key travels in the request URL query string on every documented endpoint. Query\n    strings are routinely written to proxy, gateway, CDN and browser-history logs, so the\n    credential has a materially larger exposure surface than a header-borne one.\n  remedy: Accept the key in an Authorization or X-API-Key request header.\n- id: no-scopes\n  severity: medium\n  finding: >-\n    A single account key authorizes every operation — placing calls, sending SMS to customers,\n    and mutating PowerLists — with no scope, role or capability restriction.\n  remedy: Introduce scoped keys, or an OAuth 2.0 client-credentials flow with scopes.\n- id: no-rotation-policy\n  severity: medium\n  finding: No published key-rotation, expiry, or multi-key policy; one key per account.\n  remedy: Support multiple concurrent named keys so a key can be rotated without downtime.\n- id: parameter-name-inconsistency\n  severity: low\n  finding:\
  \ >-\n    `apikey` on the Event and Webhook Management APIs, `apiKey` on the Agent Status API.\n  remedy: Accept both casings, or normalise to one and document the alias.\n- id: no-openid-connect\n  severity: informational\n  finding: >-\n    No /.well-known/openid-configuration or /.well-known/oauth-authorization-server is served on\n    any Kixie host (probed 2026-08-12 — see well-known/kixie-well-known.yml).\n\ntransport:\n  tls_required: true\n  documented_content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kixie/refs/heads/main/authentication/kixie-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Sales Engagement
- Voice
- Telephony
- SMS
- Messaging
- Contact Center
- Power Dialer
- CRM
- Webhook
- Communications
- Revenue Operations
---
