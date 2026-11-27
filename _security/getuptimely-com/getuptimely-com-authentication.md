---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getuptimely-com-alerts-api-openapi.yml
  format: yaml
  label: Uptimely Alerts API
  slug: getuptimely-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-alerts-api-openapi.yml
- filename: getuptimely-com-incidents-api-openapi.yml
  format: yaml
  label: Uptimely Incidents API
  slug: getuptimely-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-incidents-api-openapi.yml
- filename: getuptimely-com-monitors-api-openapi.yml
  format: yaml
  label: Uptimely Monitors API
  slug: getuptimely-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-monitors-api-openapi.yml
- filename: getuptimely-com-on-call-api-openapi.yml
  format: yaml
  label: Uptimely On Call API
  slug: getuptimely-com-on-call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-on-call-api-openapi.yml
- filename: getuptimely-com-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: Uptimely Scheduled Maintenances API
  slug: getuptimely-com-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-scheduled-maintenances-api-openapi.yml
- filename: getuptimely-com-status-pages-api-openapi.yml
  format: yaml
  label: Uptimely Status Pages API
  slug: getuptimely-com-status-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-status-pages-api-openapi.yml
- filename: getuptimely-com-usage-api-openapi.yml
  format: yaml
  label: Uptimely Usage API
  slug: getuptimely-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-usage-api-openapi.yml
- filename: getuptimely-com-webhooks-api-openapi.yml
  format: yaml
  label: Uptimely Webhooks API
  slug: getuptimely-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods published for Uptimely APIs
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Uptimely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uptimely declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Uptimely
provider_slug: getuptimely-com
scheme_count: 4
schemes:
- evidence: 'Create a key under Settings → API Keys → Public API keys in your project (keys are shown once and stored hashed), then send it as a Bearer token: curl https://app.getuptimely.com/v1/monitors \ -H "Authorization: Bearer $UPTIMELY_API_KEY "'
  header: Authorization
  how_to_obtain: Create a public API key in the project Settings → API Keys → Public API keys page.
  location: header
  name: Public REST API
  type: http-bearer
- evidence: 'It authenticates with a legacy project API key (the "API Keys" card under Settings → API Keys, below the public keys — the same key class the MCP tools take), sent as Authorization: Bearer … .'
  header: Authorization
  how_to_obtain: Create a legacy project API key in Settings → API Keys.
  location: header
  name: Prometheus scrape endpoint
  type: http-bearer
- evidence: Authenticate with a telemetry ingestion key in the x-uptimely-ingestion-key header (x-uptimely-service-token and x-uptimely-token are accepted as aliases, for OTel distros that send one of those).
  header: x-uptimely-ingestion-key
  how_to_obtain: Create a telemetry ingestion key (method not detailed on the page).
  location: header
  name: OpenTelemetry ingestion
  type: apiKey
- evidence: It authenticates with OAuth 2.1 (dynamic client registration, PKCE, consent screen in the browser) and covers everything the person can do in Uptimely.
  how_to_obtain: User signs in through the browser when the first tool is used; no key is needed.
  name: MCP server
  type: oauth2
slug: getuptimely-com-authentication
source_filename: getuptimely-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getuptimely.com/docs/api
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getuptimely.com/docs/api\nsources:\n- https://getuptimely.com/docs/api\n- https://getuptimely.com/docs/api-reference/webhooks/rotateWebhookEndpointSecret\n- https://getuptimely.com/docs/getting-started\n- https://getuptimely.com/agent-setup/prompt.md\ndescription: Authentication methods published for Uptimely APIs\nschemes:\n- type: http-bearer\n  name: Public REST API\n  evidence: 'Create a key under Settings → API Keys → Public API keys in your project (keys are shown once and stored hashed), then send it as\n    a Bearer token: curl https://app.getuptimely.com/v1/monitors \\ -H \"Authorization: Bearer $UPTIMELY_API_KEY \"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a public API key in the project Settings → API Keys → Public API keys page.\n- type: http-bearer\n  name: Prometheus scrape endpoint\n  evidence: 'It authenticates with a legacy project\
  \ API key (the \"API Keys\" card under Settings → API Keys, below the public keys — the same key\n    class the MCP tools take), sent as Authorization: Bearer … .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a legacy project API key in Settings → API Keys.\n- type: apiKey\n  name: OpenTelemetry ingestion\n  evidence: Authenticate with a telemetry ingestion key in the x-uptimely-ingestion-key header (x-uptimely-service-token and x-uptimely-token\n    are accepted as aliases, for OTel distros that send one of those).\n  location: header\n  header: x-uptimely-ingestion-key\n  how_to_obtain: Create a telemetry ingestion key (method not detailed on the page).\n- type: oauth2\n  name: MCP server\n  evidence: It authenticates with OAuth 2.1 (dynamic client registration, PKCE, consent screen in the browser) and covers everything the person\n    can do in Uptimely.\n  how_to_obtain: User signs in through the browser when the first tool is used; no key is needed.\ndocs:\
  \ https://getuptimely.com/docs/api\n"
source_yaml_url: https://artifacts.apis.io/getuptimely-com/authentication/getuptimely-com-authentication.yml
summary_line: 4 schemes
tags:
- Monitoring
- Uptime
- Status Pages
- On-Call
---
