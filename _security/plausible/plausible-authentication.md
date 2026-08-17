---
api_key_in:
- header
api_specs:
- filename: plausible-customprops-api-openapi.yml
  format: yaml
  label: Plausible CustomProps API
  slug: plausible-customprops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-customprops-api-openapi.yml
- filename: plausible-events-api-openapi.yml
  format: yaml
  label: Plausible Events API
  slug: plausible-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-events-api-openapi.yml
- filename: plausible-goals-api-openapi.yml
  format: yaml
  label: Plausible Goals API
  slug: plausible-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-goals-api-openapi.yml
- filename: plausible-guests-api-openapi.yml
  format: yaml
  label: Plausible Guests API
  slug: plausible-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-guests-api-openapi.yml
- filename: plausible-query-api-openapi.yml
  format: yaml
  label: Plausible Query API
  slug: plausible-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-query-api-openapi.yml
- filename: plausible-sharedlinks-api-openapi.yml
  format: yaml
  label: Plausible SharedLinks API
  slug: plausible-sharedlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-sharedlinks-api-openapi.yml
- filename: plausible-sites-api-openapi.yml
  format: yaml
  label: Plausible Sites API
  slug: plausible-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-sites-api-openapi.yml
- filename: plausible-teams-api-openapi.yml
  format: yaml
  label: Plausible Teams API
  slug: plausible-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Plausible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plausible secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plausible
provider_slug: plausible
scheme_count: 1
schemes:
- bearerFormat: API Key
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/plausible-stats-openapi.yml
  - https://plausible.io/docs/stats-api
  type: http
  value_form: Bearer YOUR-KEY
slug: plausible-authentication
source_filename: plausible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/plausible-stats-openapi.yml\ndocs: https://plausible.io/docs/stats-api\nalso_docs:\n  - https://plausible.io/docs/sites-api\n  - https://plausible.io/docs/events-api\n  - https://plausible.io/docs/account-settings\nsummary:\n  types:\n  - http\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  header: Authorization\n  value_form: 'Bearer YOUR-KEY'\n  sources:\n  - openapi/_original/plausible-stats-openapi.yml\n  - https://plausible.io/docs/stats-api\nkey_types:\n  - name: Stats API key\n    grants: 'POST /api/v2/query and the legacy /api/v1/stats/* surface'\n    created_in: 'Account settings > API Keys > create a new Stats API key'\n    plan_required: 'Business (600 requests/hour) or Enterprise'\n    docs: https://plausible.io/docs/stats-api\n  - name: Sites API key\n    grants: 'the /api/v1/sites/* surface — sites, goals, guests,\
  \ custom properties, shared links, teams'\n    created_in: 'Account settings > API Keys > create a new Sites API key'\n    plan_required: 'Enterprise (\"Sites API is available on Enterprise plans\")'\n    docs: https://plausible.io/docs/sites-api\nunauthenticated_surfaces:\n  - surface: 'POST https://plausible.io/api/event'\n    detail: >-\n      The Events ingest endpoint takes NO credential at all. It is authorised by the\n      `domain` in the payload matching a site registered in Plausible; anything else is\n      accepted with 202 and silently dropped (x-plausible-dropped: 1). Available on all\n      plans, including free trials.\n    docs: https://plausible.io/docs/events-api\n  - surface: 'https://plausible.io/share/<domain>?auth=<token>'\n    detail: >-\n      Shared-link dashboards are authorised by a bearer-like token in the query string, not\n      by an API key. Optionally password protected. Created via upsertSharedLink.\n    docs: https://plausible.io/docs/embed-dashboard\n\
  not_supported:\n  oauth2: 'no oauth2 securityScheme; /.well-known/oauth-authorization-server probed 2026-08-13 returned 404'\n  openid_connect: '/.well-known/openid-configuration probed 2026-08-13 returned 404'\n  mutual_tls: not documented\n  scopes: >-\n    No scope or permission model is published. A key''s reach is fixed by its TYPE (Stats vs\n    Sites) at creation time — it cannot be narrowed to a single site, to read-only, or to a\n    subset of operations. A Sites API key can delete every site on the account. No\n    scopes/ artifact is written because there is no scope surface to record.\n  key_rotation: 'not documented; keys are created and revoked manually in Account settings'\n  test_keys: 'no test/live key separation — see sandbox/plausible-sandbox.yml'\naccount_security:\n  two_factor: 'supported; team owners can enforce 2FA account-wide (changelog 2025-11-05)'\n  sso: 'SAML 2.0 single sign-on on Enterprise plans (https://plausible.io/compliance) — dashboard login only, not\
  \ API authorization'\nfailure_modes:\n  - {status: 401, body: '{\"error\":\"Missing API key. Please use a valid Plausible API key as a Bearer Token.\"}', cause: 'no Authorization header', observed: '2026-08-13'}\n  - {status: 401, body: '{\"error\":\"Invalid API key or site ID. Please make sure you''re using a valid API key with access to the site you''ve requested.\"}', cause: 'bad key, wrong key type, wrong plan, or no access to site_id — all conflated into one message', observed: '2026-08-13'}\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/authentication/plausible-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Cookie-Free
- Event Tracking
- GDPR
- Goal Conversions
- Open Source
- Privacy
- Self-Hosted
- Site Management
- Web Analytics
---
