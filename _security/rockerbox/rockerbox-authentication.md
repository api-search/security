---
api_key_in:
- query
auth_types:
- tenant-identifier
- session-login
- warehouse-grant
description: 'Rockerbox publishes no OpenAPI, so this profile could not be derived mechanically (0-working/derive-authentication.py needs securitySchemes). It was read from the provider''s own documentation instead. The finding is unusual and worth stating plainly: Rockerbox''s public ingestion endpoint has NO credential at all — it is authenticated by an opaque tenant identifier in the query string, issued by a human account manager. Everything richer (dashboard, exports, warehouse shares) sits behind account provisioning, not behind a developer credential.'
kind: authentication
layout: security
method: searched
name: Rockerbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rockerbox secures its APIs with tenant-identifier, session-login, and warehouse-grant across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rockerbox
provider_slug: rockerbox
scheme_count: 5
schemes:
- description: A Rockerbox Advertiser ID passed as a query-string parameter on every POST. The docs say explicitly "You will need the following field from Rockerbox. Please ask your account manager for this field." There is no rotation, expiry, scope or signing documented.
  endpoint: https://webhooks.getrockerbox.com/webhook/data
  in: query
  name: advertiser-id
  parameter: advertiser
  risk_note: A bare tenant identifier in a URL is an identifier, not a secret — it is not a bearer credential and Rockerbox does not describe it as one. Recorded as observed; no security claim is made for it.
  rotatable: unknown
  self_service: false
  source: https://help.rockerbox.com/article/5t050dmcxv-webhooks
  surface: Conversion / marketing event ingestion
  type: apiKey
- description: Client-side tracking is bound to the account by the Pixel Source Name, the public account identifier embedded in the tag. Documented as an account ID, not a credential.
  in: script
  name: pixel-source-name
  parameter: pixel source name (account ID)
  source: https://help.rockerbox.com/article/gdeze5itjv-pixel-source-name-account-id
  surface: Onsite conversion / identify pixels
  type: tenantIdentifier
- description: Username / password session login to the Rockerbox dashboard, where users, exports and scheduled reports are managed. User administration is documented; no API-token issuance page was found.
  in: cookie
  login_url: https://app.rockerbox.com/login
  name: dashboard-login
  source: https://help.rockerbox.com/article/n58en66w7j-forgot-password-troubleshoot-login
  surface: Rockerbox application (app.rockerbox.com)
  type: session
- description: Access to the warehouse datasets is granted by the warehouse platform's own mechanism rather than by a Rockerbox credential — Snowflake data sharing, BigQuery project-level permissions, or Redshift IAM roles. Enabled by a Rockerbox representative as a paid add-on.
  name: warehouse-grant
  source: https://data-foundation.rockerbox.com/warehousing/quickstart
  surface: Data Foundation warehouse share
  type: platform-native
- description: The remote MCP server is anonymous. /.well-known/mcp.json declares "authentication":"none" and an unauthenticated initialize + tools/list handshake returned HTTP 200. Verified by probe.
  endpoint: https://data-foundation.rockerbox.com/mcp
  name: none
  surface: Data Foundation docs MCP server
  type: none
  verified: probed
slug: rockerbox-authentication
source_filename: rockerbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.rockerbox.com/article/5t050dmcxv-webhooks\ndocs: https://help.rockerbox.com/category/enoswvfeqo-setup-and-technical-documentation\ndescription: >-\n  Rockerbox publishes no OpenAPI, so this profile could not be derived mechanically\n  (0-working/derive-authentication.py needs securitySchemes). It was read from the provider's own\n  documentation instead. The finding is unusual and worth stating plainly: Rockerbox's public\n  ingestion endpoint has NO credential at all — it is authenticated by an opaque tenant identifier in\n  the query string, issued by a human account manager. Everything richer (dashboard, exports,\n  warehouse shares) sits behind account provisioning, not behind a developer credential.\nsummary:\n  types: [tenant-identifier, session-login, warehouse-grant]\n  api_key_in: [query]\n  oauth2_flows: []\n  oauth2_published: false\n  openid_connect_published: false\n  mutual_tls_published: false\n\
  \  self_service_credentials: false\nschemes:\n- name: advertiser-id\n  surface: Conversion / marketing event ingestion\n  endpoint: https://webhooks.getrockerbox.com/webhook/data\n  type: apiKey\n  in: query\n  parameter: advertiser\n  description: >-\n    A Rockerbox Advertiser ID passed as a query-string parameter on every POST. The docs say\n    explicitly \"You will need the following field from Rockerbox. Please ask your account manager for\n    this field.\" There is no rotation, expiry, scope or signing documented.\n  self_service: false\n  rotatable: unknown\n  source: https://help.rockerbox.com/article/5t050dmcxv-webhooks\n  risk_note: >-\n    A bare tenant identifier in a URL is an identifier, not a secret — it is not a bearer credential\n    and Rockerbox does not describe it as one. Recorded as observed; no security claim is made for it.\n- name: pixel-source-name\n  surface: Onsite conversion / identify pixels\n  type: tenantIdentifier\n  in: script\n  parameter: pixel source\
  \ name (account ID)\n  description: >-\n    Client-side tracking is bound to the account by the Pixel Source Name, the public account\n    identifier embedded in the tag. Documented as an account ID, not a credential.\n  source: https://help.rockerbox.com/article/gdeze5itjv-pixel-source-name-account-id\n- name: dashboard-login\n  surface: Rockerbox application (app.rockerbox.com)\n  type: session\n  in: cookie\n  description: >-\n    Username / password session login to the Rockerbox dashboard, where users, exports and scheduled\n    reports are managed. User administration is documented; no API-token issuance page was found.\n  login_url: https://app.rockerbox.com/login\n  source: https://help.rockerbox.com/article/n58en66w7j-forgot-password-troubleshoot-login\n- name: warehouse-grant\n  surface: Data Foundation warehouse share\n  type: platform-native\n  description: >-\n    Access to the warehouse datasets is granted by the warehouse platform's own mechanism rather than\n    by a Rockerbox\
  \ credential — Snowflake data sharing, BigQuery project-level permissions, or\n    Redshift IAM roles. Enabled by a Rockerbox representative as a paid add-on.\n  source: https://data-foundation.rockerbox.com/warehousing/quickstart\n- name: none\n  surface: Data Foundation docs MCP server\n  endpoint: https://data-foundation.rockerbox.com/mcp\n  type: none\n  description: >-\n    The remote MCP server is anonymous. /.well-known/mcp.json declares \"authentication\":\"none\" and an\n    unauthenticated initialize + tools/list handshake returned HTTP 200. Verified by probe.\n  verified: probed\ngaps:\n- No OAuth 2.0, OpenID Connect or mutual TLS is published on any Rockerbox surface.\n- No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource is served (all 404 / soft-200).\n- No developer-facing API key issuance, rotation or scope documentation was found.\n- No signing, HMAC or replay protection is documented for the ingestion webhook.\nx-evidence:\n- {url: 'https://help.rockerbox.com/article/5t050dmcxv-webhooks',\
  \ http_status: 200, fetched: '2026-08-13'}\n- {url: 'https://data-foundation.rockerbox.com/warehousing/quickstart.md', http_status: 200, fetched: '2026-08-13'}\n- {url: 'https://data-foundation.rockerbox.com/.well-known/mcp.json', http_status: 200, fetched: '2026-08-13'}\n- {url: 'https://app.rockerbox.com/login', http_status: 200, fetched: '2026-08-13'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockerbox/refs/heads/main/authentication/rockerbox-authentication.yml
summary_line: tenant-identifier/session-login/warehouse-grant · 5 schemes
tags:
- Marketing Attribution
- Multi-Touch Attribution
- Marketing Mix Modeling
- Incrementality Testing
- Media Spend
- Customer Journeys
- Marketing Analytics
- Data Warehousing
- Conversion Tracking
- Webhook
---
