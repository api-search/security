---
api_key_in:
- header
- query
api_specs:
- filename: peopledatalabs-autocomplete-api-openapi.yml
  format: yaml
  label: People Data Labs Autocomplete API
  slug: peopledatalabs-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-autocomplete-api-openapi.yml
- filename: peopledatalabs-cleaner-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Cleaner Endpoints API
  slug: peopledatalabs-cleaner-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-cleaner-endpoints-api-openapi.yml
- filename: peopledatalabs-company-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Company Endpoints API
  slug: peopledatalabs-company-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-company-endpoints-api-openapi.yml
- filename: peopledatalabs-ip-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs IP Enrichment API
  slug: peopledatalabs-ip-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-ip-enrichment-api-openapi.yml
- filename: peopledatalabs-job-title-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs Job Title Enrichment API
  slug: peopledatalabs-job-title-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-job-title-enrichment-api-openapi.yml
- filename: peopledatalabs-person-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Person Endpoints API
  slug: peopledatalabs-person-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-person-endpoints-api-openapi.yml
- filename: peopledatalabs-skill-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs Skill Enrichment API
  slug: peopledatalabs-skill-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-skill-enrichment-api-openapi.yml
- filename: peopledatalabs-subscription-api-openapi.yml
  format: yaml
  label: People Data Labs Subscription API
  slug: peopledatalabs-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-subscription-api-openapi.yml
- filename: peopledatalabs-preview-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs Preview Enrichment API
  slug: peopledatalabs-preview-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-preview-enrichment-api-openapi.yml
- filename: peopledatalabs-subject-request-api-openapi.yml
  format: yaml
  label: People Data Labs Subject Request API
  slug: peopledatalabs-subject-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-subject-request-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Peopledatalabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: People Data Labs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: People Data Labs
provider_slug: peopledatalabs
scheme_count: 2
schemes:
- description: The documented and recommended placement. The published OpenAPI declares the header as X-API-Key; the documentation and every SDK example use X-Api-Key. HTTP header names are case-insensitive, so both work.
  in: header
  name: APIKeyHeader
  parameterName: X-Api-Key
  recommended: true
  sources:
  - openapi/_original/peopledatalabs-openapi.yml
  - openapi/_original/peopledatalabs-docs-openapi.json
  - https://docs.peopledatalabs.com/docs/authentication
  type: apiKey
- description: Documented alternative — the key may be passed in the query string (?api_key=...). Not declared in either OpenAPI document. It works, and it puts a long-lived credential in URLs, logs and referrers; prefer the header.
  in: query
  name: APIKeyQuery
  parameterName: api_key
  recommended: false
  sources:
  - https://docs.peopledatalabs.com/docs/authentication
  type: apiKey
slug: peopledatalabs-authentication
source_filename: peopledatalabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.peopledatalabs.com/docs/authentication\nderived_from:\n- openapi/_original/peopledatalabs-openapi.yml\n- openapi/_original/peopledatalabs-docs-openapi.json\ndocs: https://docs.peopledatalabs.com/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  scopes: none\n  note: >-\n    One credential, three placements. Every People Data Labs endpoint — including the\n    sandbox host and the subscription/webhook management surface — is authenticated by a\n    single account API key. There are no scopes, no OAuth, no per-endpoint permissions and\n    no token exchange, so an agent handed a PDL key holds the full account: every dataset\n    the plan includes, every credit on the account, and the ability to create, change and\n    delete webhook subscriptions.\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameterName: X-Api-Key\n  recommended:\
  \ true\n  description: >-\n    The documented and recommended placement. The published OpenAPI declares the header as\n    X-API-Key; the documentation and every SDK example use X-Api-Key. HTTP header names are\n    case-insensitive, so both work.\n  sources:\n  - openapi/_original/peopledatalabs-openapi.yml\n  - openapi/_original/peopledatalabs-docs-openapi.json\n  - https://docs.peopledatalabs.com/docs/authentication\n- name: APIKeyQuery\n  type: apiKey\n  in: query\n  parameterName: api_key\n  recommended: false\n  description: >-\n    Documented alternative — the key may be passed in the query string\n    (?api_key=...). Not declared in either OpenAPI document. It works, and it puts a\n    long-lived credential in URLs, logs and referrers; prefer the header.\n  sources:\n  - https://docs.peopledatalabs.com/docs/authentication\nkey_management:\n  issuance: https://dashboard.peopledatalabs.com\n  rotation: >-\n    Self-serve rotation is not documented. To request a new key or delete\
  \ an existing one\n    the docs direct customers to their account manager or support@peopledatalabs.com.\n  expiry: not documented\n  scopes: none\n  environments:\n    note: >-\n      The same key authenticates both the production host and\n      sandbox.api.peopledatalabs.com. There is no separate test key and no key prefix that\n      distinguishes test from live.\ntransport:\n  https_required: true\n  note: Requests over plain HTTP fail.\nfailure_modes:\n- status: 401\n  type: authentication_error\n  cause: missing or invalid key\nsdk_support:\n- language: python\n  snippet: 'PDLPY(api_key=\"YOUR API KEY\")'\n- language: javascript\n  snippet: 'new PDLJS({ apiKey: \"YOUR API KEY\" })'\n- language: ruby\n  snippet: 'Peopledatalabs.api_key = \"YOUR API KEY\"'\n- language: go\n  snippet: 'pdl.New(apiKey)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/authentication/peopledatalabs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data Enrichment
- Web Intelligence
- Person Data
- Company Data
- B2B Data
- Contact Discovery
- Reference Data
- Firmographics
- Identity Resolution
---
