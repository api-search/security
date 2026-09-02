---
api_key_in:
- query
- body
api_specs:
- filename: smartlead-ai-campaign-statistics-api-openapi.yml
  format: yaml
  label: Smartlead Campaign Statistics API
  slug: smartlead-ai-campaign-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-campaign-statistics-api-openapi.yml
- filename: smartlead-ai-campaigns-api-openapi.yml
  format: yaml
  label: Smartlead Campaigns API
  slug: smartlead-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-campaigns-api-openapi.yml
- filename: smartlead-ai-analytics-api-openapi.yml
  format: yaml
  label: Smartlead Analytics API
  slug: smartlead-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-analytics-api-openapi.yml
- filename: smartlead-ai-authentication-api-openapi.yml
  format: yaml
  label: Smartlead Authentication API
  slug: smartlead-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-authentication-api-openapi.yml
- filename: smartlead-ai-email-accounts-api-openapi.yml
  format: yaml
  label: Smartlead Email Accounts API
  slug: smartlead-ai-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-email-accounts-api-openapi.yml
- filename: smartlead-ai-leads-api-openapi.yml
  format: yaml
  label: Smartlead Leads API
  slug: smartlead-ai-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-leads-api-openapi.yml
- filename: smartlead-ai-master-inbox-api-openapi.yml
  format: yaml
  label: Smartlead Master Inbox API
  slug: smartlead-ai-master-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-master-inbox-api-openapi.yml
- filename: smartlead-ai-smart-delivery-api-openapi.yml
  format: yaml
  label: Smartlead Smart Delivery API
  slug: smartlead-ai-smart-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-smart-delivery-api-openapi.yml
- filename: smartlead-ai-smart-senders-api-openapi.yml
  format: yaml
  label: Smartlead Smart Senders API
  slug: smartlead-ai-smart-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-smart-senders-api-openapi.yml
- filename: smartlead-ai-utilities-api-openapi.yml
  format: yaml
  label: Smartlead Utilities API
  slug: smartlead-ai-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-utilities-api-openapi.yml
- filename: smartlead-ai-webhooks-api-openapi.yml
  format: yaml
  label: Smartlead Webhooks API
  slug: smartlead-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Smartlead Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smartlead secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smartlead
provider_slug: smartlead-ai
scheme_count: 1
schemes:
- applied: 'globally — the spec declares a root-level security requirement of [{ApiKeyAuth: []}]'
  description: 'Your SmartLead API key. You can generate this from your dashboard under Settings > API Keys.


    Include this as a query parameter in all API requests:

    ```

    ?api_key=YOUR_API_KEY

    ```'
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/smartlead-ai-campaign-statistics-api-openapi.yml
  - openapi/smartlead-ai-campaigns-api-openapi.yml
  - openapi/smartlead-ai-openapi.yml
  type: apiKey
slug: smartlead-ai-authentication
source_filename: smartlead-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/smartlead-ai-openapi.yml\ndocs: https://api.smartlead.ai/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - body\n  oauth2_flows: []\n  scopes: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: |-\n    Your SmartLead API key. You can generate this from your dashboard under Settings > API Keys.\n\n    Include this as a query parameter in all API requests:\n    ```\n    ?api_key=YOUR_API_KEY\n    ```\n  applied: >-\n    globally — the spec declares a root-level security requirement of [{ApiKeyAuth: []}]\n  sources:\n  - openapi/smartlead-ai-campaign-statistics-api-openapi.yml\n  - openapi/smartlead-ai-campaigns-api-openapi.yml\n  - openapi/smartlead-ai-openapi.yml\nalternate_transport:\n  in: body\n  parameter: api_key\n  note: >-\n    The auth docs state that on POST/PATCH the key may instead be included as an `api_key` field in\n    the\
  \ JSON request body. This is documented but is NOT modelled in the OpenAPI, which declares\n    only the query-parameter scheme.\nissuance:\n  console: https://app.smartlead.ai\n  path: Profile icon -> Settings -> API Keys -> Generate New API Key\n  shown_once: true\n  rotation: >-\n    Keys can be regenerated from the dashboard. Agency accounts can additionally create, list,\n    reset and revoke per-client keys (see the CLI `clients` command group).\n  agency_scoped_keys: true\nfailure:\n  status: 401\n  body_shape: '{\"success\": false, ...}'\n  detail: errors/smartlead-ai-problem-types.yml\nrisk_notes:\n- >-\n  The credential is carried in the URL query string on every request, including GETs. Query\n  strings are routinely recorded in proxy, CDN, load-balancer and web-server access logs, in\n  browser history, and in Referer headers — so the key is exposed anywhere the URL is logged.\n  SmartLead documents no header-based alternative.\n- >-\n  Keys are account-wide bearer credentials\
  \ with no scopes and no least-privilege model: any key\n  can read the master inbox, send email, import leads and manage mailboxes. SmartLead's own docs\n  say \"your API key carries many privileges\".\n- >-\n  The one mitigation SmartLead does offer is agency key segmentation — a separate key per client\n  workspace, revocable independently.\nnot_supported:\n- oauth2\n- openIdConnect\n- mutualTLS\n- http bearer\n- scopes / granular permissions\n- key expiry or TTL (none documented)\nrelated:\n  conventions: conventions/smartlead-ai-conventions.yml\n  conformance: conformance/smartlead-ai-conformance.yml\nx-evidence:\n- url: https://api.smartlead.ai/authentication\n  http_status: 200\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/authentication/smartlead-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cold Email
- Outbound
- Sales
- Deliverability
- Email Warm-up
- Automation
- Sequences
---
