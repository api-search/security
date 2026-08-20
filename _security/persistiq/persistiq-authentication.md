---
api_key_in:
- header
api_specs:
- filename: persistiq-campaigns-api-openapi.yml
  format: yaml
  label: PersistIQ Campaigns API
  slug: persistiq-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-campaigns-api-openapi.yml
- filename: persistiq-do-not-contact-domains-api-openapi.yml
  format: yaml
  label: PersistIQ Do Not Contact Domains API
  slug: persistiq-do-not-contact-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-do-not-contact-domains-api-openapi.yml
- filename: persistiq-events-api-openapi.yml
  format: yaml
  label: PersistIQ Events API
  slug: persistiq-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-events-api-openapi.yml
- filename: persistiq-lead-fields-api-openapi.yml
  format: yaml
  label: PersistIQ Lead Fields API
  slug: persistiq-lead-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-lead-fields-api-openapi.yml
- filename: persistiq-lead-statuses-api-openapi.yml
  format: yaml
  label: PersistIQ Lead Statuses API
  slug: persistiq-lead-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-lead-statuses-api-openapi.yml
- filename: persistiq-leads-api-openapi.yml
  format: yaml
  label: PersistIQ Leads API
  slug: persistiq-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-leads-api-openapi.yml
- filename: persistiq-users-api-openapi.yml
  format: yaml
  label: PersistIQ Users API
  slug: persistiq-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-users-api-openapi.yml
- filename: persistiq-api-v1-openapi.json
  format: json
  label: PersistIQ Tags API
  slug: persistiq-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-api-v1-openapi.json
- filename: persistiq-api-v1-openapi.json
  format: json
  label: PersistIQ Replies API
  slug: persistiq-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-api-v1-openapi.json
- filename: persistiq-api-v1-openapi.json
  format: json
  label: PersistIQ Webhook Plugin API
  slug: persistiq-webhook-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-api-v1-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Persistiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: PersistIQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PersistIQ
provider_slug: persistiq
scheme_count: 1
schemes:
- applied: global
  applied_note: 'Declared at the document root as `security: [{api_key: []}]`, so it applies to all 21 operations; no operation overrides or opts out.'
  description: Company-wide API key. Grants read and write access to all users' data within the company. Include it in the header of every request. PersistIQ's own OpenAPI states it is "API key found in Settings > Integrations > API Key".
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/persistiq-api-v1-openapi.json
  - openapi/persistiq-openapi.yml
  type: apiKey
slug: persistiq-authentication
source_filename: persistiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.persistiq.com/api-docs/v1/swagger.json\ndocs: https://apidocs.persistiq.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: none\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    Company-wide API key. Grants read and write access to all users' data within\n    the company. Include it in the header of every request. PersistIQ's own\n    OpenAPI states it is \"API key found in Settings > Integrations > API Key\".\n  applied: global\n  applied_note: >-\n    Declared at the document root as `security: [{api_key: []}]`, so it applies\n    to all 21 operations; no operation overrides or opts out.\n  sources:\n  - openapi/persistiq-api-v1-openapi.json\n  - openapi/persistiq-openapi.yml\nkey_management:\n  location: PersistIQ app, Settings > Integrations > API Key\n  rotation: not documented\n  per_user_keys: false\n  expiry:\
  \ none documented\n  notes: >-\n    One key per company, not per user. There is no scope surface, no key\n    rotation endpoint, and no way to issue a reduced-privilege key — any holder\n    of the key can read and write every user's prospects, campaigns, replies and\n    webhook destinations. That is the single most important fact for anyone\n    handing this key to an agent.\nunauthenticated_behaviour:\n  method: probed\n  fetched: '2026-08-13'\n  request: GET https://api.persistiq.com/v1/users\n  http_status: 401\n  body: >-\n    {\"status\":\"error\",\"error\":{\"reason\":\"unauthorized\",\"message\":\"Failed to find\n    api key: .  Did you set header 'x-api-key' ...}}\n  notes: >-\n    A missing key returns 401 with the standard error envelope and a `reason` of\n    `unauthorized`. Rate-limit headers are still returned on the 401.\noauth: false\nmtls: false\nopenid_connect: false\nnotes: >-\n  Upgraded from derived to searched on 2026-08-13 against PersistIQ's own\n  OpenAPI 3.0.1\
  \ document, which names the scheme `api_key` (an earlier round\n  guessed `ApiKeyAuth` from the reference prose). No OAuth 2.0, OIDC or mTLS\n  surface exists, so no scopes/ artifact is emitted — there is nothing to scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/authentication/persistiq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Sales Engagement
- Sales
- Outbound
- Email Outreach
- CRM
- Lead Management
- Marketing
- Webhook
- SEP
---
