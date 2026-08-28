---
api_key_in: []
api_specs:
- filename: hyperdx-external-api-openapi.json
  format: json
  label: HyperDX External API
  slug: hyperdx-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperdx/refs/heads/main/openapi/hyperdx-external-api-openapi.json
auth_types:
- http
description: One credential, one scheme, across every HyperDX surface. The REST API (v1 and v2), the MCP server and the CLI all authenticate with a personal API access key presented as an HTTP Bearer token. There is no OAuth, no OpenID Connect, no mTLS, no scopes and no service-account concept — the key carries whatever the person it belongs to can do in their team.
kind: authentication
layout: security
method: searched
name: Hyperdx Authentication
name_suffix: Authentication
oauth_flows: []
overview: HyperDX secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HyperDX
provider_slug: hyperdx
scheme_count: 1
schemes:
- applies_to:
  - HyperDX External API v2 (all 39 operations — declared as a global `security` requirement)
  - HyperDX Cloud API v1 (documented on hyperdx.io/docs/api)
  - HyperDX MCP server at /api/mcp (Streamable HTTP, Authorization header)
  - '@hyperdx/cli (hdx auth login stores the credential)'
  bearerFormat: API Key
  format: 'Authorization: Bearer <personal API access key>'
  header: Authorization
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/hyperdx-external-api-openapi.json
  - https://www.hyperdx.io/docs/api/alerts
  - https://github.com/hyperdxio/hyperdx/blob/main/MCP.md
  type: http
slug: hyperdx-authentication
source_filename: hyperdx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/hyperdx-external-api-openapi.json + https://www.hyperdx.io/docs/api/alerts + https://github.com/hyperdxio/hyperdx/blob/main/MCP.md\ndocs: https://www.hyperdx.io/docs/api/alerts\nname: HyperDX Authentication\ndescription: >-\n  One credential, one scheme, across every HyperDX surface. The REST API (v1 and v2), the MCP\n  server and the CLI all authenticate with a personal API access key presented as an HTTP Bearer\n  token. There is no OAuth, no OpenID Connect, no mTLS, no scopes and no service-account concept —\n  the key carries whatever the person it belongs to can do in their team.\nsummary:\n  types:\n  - http\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  api_key_header: false\n  scopes: false\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  header: Authorization\n  format: 'Authorization: Bearer <personal API access key>'\n  sources:\n  - openapi/hyperdx-external-api-openapi.json\n\
  \  - https://www.hyperdx.io/docs/api/alerts\n  - https://github.com/hyperdxio/hyperdx/blob/main/MCP.md\n  applies_to:\n  - HyperDX External API v2 (all 39 operations — declared as a global `security` requirement)\n  - HyperDX Cloud API v1 (documented on hyperdx.io/docs/api)\n  - HyperDX MCP server at /api/mcp (Streamable HTTP, Authorization header)\n  - '@hyperdx/cli (hdx auth login stores the credential)'\ncredential:\n  name: Personal API access key\n  where: HyperDX UI > Team Settings > API keys > Personal API access key\n  prefix: null\n  prefix_note: No documented key prefix, so a leaked key is not identifiable by shape.\n  rotation:\n    supported: true\n    since: 2.36.0\n    since_date: '2026-08-21'\n    note: >-\n      Before release 2.36.0 the personal API access key was fixed for the life of the account and\n      could not be rotated. Any deployment older than 2026-08-21 has no rotation path.\n  expiry: none documented\n  scoping: >-\n    Team-scoped and personal. A 403 means\
  \ the key authenticated but the team or resource is out of\n    reach; there is no narrower permission model to express in the request.\ningestion_credential:\n  name: Ingestion API key\n  distinct_from_management_key: true\n  note: >-\n    Telemetry ingestion into the OpenTelemetry collector uses a separate auto-generated ingestion\n    API key, sent with OTLP data — not the personal access key used for the management API. The\n    ClickStack collector distribution pulls its OTLP endpoint configuration over OpAMP.\nenterprise:\n  saml_sso: true\n  saml_note: >-\n    SAML SSO is an Enterprise-tier feature for logging into the product. It governs human sign-in,\n    not API authentication — API calls are still Bearer key.\n  oss_note: >-\n    The open-source build has no SSO and no Slack/PagerDuty OAuth; the OSS/Cloud comparison page\n    lists alert delivery there as webhooks only.\ngaps:\n- No OAuth 2.0 or OIDC, so no delegated authorization and no third-party app model.\n- No scopes\
  \ or permissions, so a key cannot be narrowed to read-only. An agent handed a key to run\n  clickstack_search can also call clickstack_delete_dashboard.\n- No key prefix and no documented expiry.\nevidence:\n- url: https://www.hyperdx.io/docs/api/alerts\n  status: 200\n- url: https://api.hyperdx.io/api/v1/alerts\n  status: 401\n  note: Unauthenticated GET returns 401 \"Unauthorized\" — confirms the scheme is enforced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperdx/refs/heads/main/authentication/hyperdx-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Observability
- Monitoring
- Logging
- Tracing
- Metrics
- OpenTelemetry
- ClickHouse
- Open Source
- Alerting
- Dashboards
- Session Replay
- Developer Tools
- Agents
---
