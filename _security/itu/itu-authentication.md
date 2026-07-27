---
api_key_in:
- query
api_specs:
- filename: itu-datahub-openapi.yml
  format: yaml
  label: ITU DataHub API
  slug: itu-datahub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/openapi/itu-datahub-openapi.yml
- filename: itu-proximity-openapi.yml
  format: yaml
  label: ITU Proximity to Fibre Node API
  slug: itu-proximity-to-fibre-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/openapi/itu-proximity-openapi.yml
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Itu Authentication
name_suffix: Authentication
oauth_flows: []
overview: ITU secures its APIs with none and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ITU
provider_slug: itu
scheme_count: 2
schemes:
- apis:
  - ITU DataHub API
  description: 'The ITU DataHub API requires no credential of any kind. Confirmed 2026-07-26: HTTP 200 on /v2/country/all, /v2/region/all, /v2/dictionaries/getcategories, /v2/umc/topic/all, /v2/idi/dashboard/version and /v2/methodology/dataset with no API key, no Authorization header, no Referer and no Origin. The service returns `access-control-allow-origin: *` and an OPTIONS preflight advertising `access-control-allow-methods: OPTIONS,GET`, so it is callable directly from a browser.'
  name: anonymous
  sources:
  - openapi/itu-datahub-openapi.yml
  type: none
- apis:
  - ITU Proximity to Fibre Node API
  description: Azure Functions function key on the ITU Proximity to Fibre Node API. ITU embeds a working key per route in its public web client at https://bbmaps.itu.int/web10km/, so the surface is effectively open — there is no registration, no self-service key issuance, no scope model and no documented rotation policy. A missing or invalid `code` returns HTTP 401 with an empty body (confirmed 2026-07-26).
  in: query
  name: functionKey
  parameter: code
  sources:
  - openapi/itu-proximity-openapi.yml
  type: apiKey
slug: itu-authentication
source_filename: itu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/itu-datahub-openapi.yml, openapi/itu-proximity-openapi.yml\nprobe: true\nprobed: '2026-07-26'\nnote: >-\n  ITU publishes no authentication documentation of any kind — there is no developer portal, no\n  signup, no key issuance, and no terms of programmatic use. This profile is derived from the two\n  OpenAPI descriptions in this repo plus live anonymous probes of both surfaces.\nsummary:\n  types:\n  - none\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  registration_required: false\n  signup_url: null\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    The ITU DataHub API requires no credential of any kind. Confirmed 2026-07-26: HTTP 200 on\n    /v2/country/all, /v2/region/all, /v2/dictionaries/getcategories, /v2/umc/topic/all,\n    /v2/idi/dashboard/version and /v2/methodology/dataset with no API key, no Authorization header,\n    no Referer and no Origin. The service returns `access-control-allow-origin:\
  \ *` and an OPTIONS\n    preflight advertising `access-control-allow-methods: OPTIONS,GET`, so it is callable directly\n    from a browser.\n  apis:\n  - ITU DataHub API\n  sources:\n  - openapi/itu-datahub-openapi.yml\n- name: functionKey\n  type: apiKey\n  in: query\n  parameter: code\n  description: >-\n    Azure Functions function key on the ITU Proximity to Fibre Node API. ITU embeds a working key\n    per route in its public web client at https://bbmaps.itu.int/web10km/, so the surface is\n    effectively open — there is no registration, no self-service key issuance, no scope model and no\n    documented rotation policy. A missing or invalid `code` returns HTTP 401 with an empty body\n    (confirmed 2026-07-26).\n  apis:\n  - ITU Proximity to Fibre Node API\n  sources:\n  - openapi/itu-proximity-openapi.yml\nabsent:\n- oauth2\n- openIdConnect\n- mutualTLS\n- http-bearer\n- http-basic\n- CIBA\nevidence:\n- source: https://api.datahub.itu.int/v2/country/all\n  status: 200\n  note:\
  \ anonymous GET, no headers sent\n- source: https://api.datahub.itu.int/v2/nosuchroute\n  status: 403\n  note: >-\n    AWS API Gateway {\"message\":\"Missing Authentication Token\"} on unrouted paths. This is a routing\n    artefact, not an auth requirement — every configured route answers anonymously.\n- source: https://bbmaps.itu.int/functionproximity/route-calcdistancetonode\n  status: 401\n  note: POST with no ?code= parameter; empty body\n- source: https://bbmaps.itu.int/functionproximity/route-calcdistancetonode?code=bogus\n  status: 401\n  note: POST with an invalid key; empty body\n- source: https://www.itu.int/.well-known/openid-configuration\n  status: 404\n  note: no OIDC discovery document on any ITU host\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/authentication/itu-authentication.yml
summary_line: none/apiKey · 2 schemes
tags:
- Telecommunications
- Global
- Regulator
- Standards
- Spectrum
- Satellite
- Broadband
- ICT Statistics
- Open Data
- United Nations
---
