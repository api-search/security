---
api_key_in: []
api_specs:
- filename: mydentify-public-api-directories-api-openapi.yml
  format: yaml
  label: Mydentify Public API Directories API
  slug: mydentify-public-api-directories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-directories-api-openapi.yml
- filename: mydentify-public-api-directories-json-api-openapi.yml
  format: yaml
  label: Mydentify Public API Directories.json API
  slug: mydentify-public-api-directories-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-directories-json-api-openapi.yml
- filename: mydentify-public-api-imports-api-openapi.yml
  format: yaml
  label: Mydentify Public API Imports API
  slug: mydentify-public-api-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-imports-api-openapi.yml
- filename: mydentify-public-api-leaderboards-api-openapi.yml
  format: yaml
  label: Mydentify Public API Leaderboards API
  slug: mydentify-public-api-leaderboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-leaderboards-api-openapi.yml
- filename: mydentify-public-api-leaderboards-json-api-openapi.yml
  format: yaml
  label: Mydentify Public API Leaderboards.json API
  slug: mydentify-public-api-leaderboards-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-leaderboards-json-api-openapi.yml
- filename: mydentify-public-api-product-categories-json-api-openapi.yml
  format: yaml
  label: Mydentify Public API Product Categories.json API
  slug: mydentify-public-api-product-categories-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-product-categories-json-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Mydentify Public Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mydentify Public API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Mydentify Public API
provider_slug: mydentify-public-api
scheme_count: 0
schemes: []
slug: mydentify-public-api-authentication
source_filename: mydentify-public-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/mydentify-public-api-openapi-original.json\ndocs: https://mydentify.com/developers\nsummary:\n  types: []\n  model: anonymous\n  api_key_in: []\n  oauth2_flows: []\n  detail: >-\n    Mydentify's public API is deliberately keyless. The OpenAPI 3.1 document declares a top-level\n    `security: []` and defines no `components.securitySchemes`; the developer guide states \"No API\n    key required — public read routes work without a token, login, or paid plan.\" This applies to\n    the write surface too: the diagnostic/submission workflow (POST /api/imports*) is\n    unauthenticated, with the Idempotency-Key header and the durable import id acting as the\n    only client-held identifiers.\nschemes: []\ntransport:\n  https_required: true\n  hsts: true\n  hsts_max_age: 31536000\n  tls_version: TLSv1.3\n  cors:\n    enabled: true\n    allow_origins: ['*']\n    scope: directory JSON endpoints\n    source: openapi x-cors extension\n\
  authorization_model:\n  public_read: unrestricted\n  writes:\n    surface: POST /api/imports, /api/imports/{id}/{retry,manual-review,goals,verify-badge}\n    control: >-\n      No credential. Access to an import is bearer-by-URL — knowledge of the UUID import id\n      returned in ImportAccepted.statusUrl / eventsUrl. Publication is additionally gated by an\n      out-of-band proof: Mydentify verifies a followed backlink or the official listing badge on\n      the submitted page before a free listing goes live.\n    escalation: POST /api/imports/{id}/verify-badge, POST /api/imports/{id}/manual-review\n  agent_boundaries:\n    source: https://mydentify.com/ai.txt\n    read_only: no user confirmation required\n    external_actions: >-\n      Submission, intent confirmation, account changes, payment and sponsorship require explicit\n      user approval.\n  excluded_from_public_api: ['/admin/*', '/dashboard/*', '/diagnostics/*', '/claim/*', authenticated responses, billing data]\ngaps:\n \
  \ - No authenticated tier is published, so there is no documented way to raise limits, claim a\n    listing programmatically, or read private diagnostic sessions via the API.\n  - There is no rate-limit contract to accompany the anonymous write surface; the only throttle\n    signal in the spec is a 429 on the retry operation.\nx-evidence:\n  fetched: '2026-08-09'\n  urls:\n    - {url: 'https://mydentify.com/openapi.json', http_status: 200}\n    - {url: 'https://mydentify.com/developers', http_status: 200}\n    - {url: 'https://mydentify.com/api/imports/dry-run', http_status: 200, note: 'anonymous POST accepted, returned a DryRunResult'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/authentication/mydentify-public-api-authentication.yml
summary_line: 0 schemes
tags:
- product discovery
- startup directories
- leaderboards
- research
- SaaS
- developer tools
- agent-native
- llms.txt
- agent skills
- directories
---
