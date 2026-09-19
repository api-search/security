---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cheniere-energy-capacity-api-openapi.yml
  format: yaml
  label: Cheniere Energy Capacity API
  slug: cheniere-energy-capacity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-capacity-api-openapi.yml
- filename: cheniere-energy-discovery-api-openapi.yml
  format: yaml
  label: Cheniere Energy Discovery API
  slug: cheniere-energy-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-discovery-api-openapi.yml
- filename: cheniere-energy-documents-api-openapi.yml
  format: yaml
  label: Cheniere Energy Documents API
  slug: cheniere-energy-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-documents-api-openapi.yml
- filename: cheniere-energy-gas-quality-api-openapi.yml
  format: yaml
  label: Cheniere Energy Gas Quality API
  slug: cheniere-energy-gas-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-gas-quality-api-openapi.yml
- filename: cheniere-energy-imbalances-api-openapi.yml
  format: yaml
  label: Cheniere Energy Imbalances API
  slug: cheniere-energy-imbalances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-imbalances-api-openapi.yml
- filename: cheniere-energy-index-of-customers-api-openapi.yml
  format: yaml
  label: Cheniere Energy Index of Customers API
  slug: cheniere-energy-index-of-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-index-of-customers-api-openapi.yml
- filename: cheniere-energy-notices-api-openapi.yml
  format: yaml
  label: Cheniere Energy Notices API
  slug: cheniere-energy-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-notices-api-openapi.yml
- filename: cheniere-energy-reference-data-api-openapi.yml
  format: yaml
  label: Cheniere Energy Reference Data API
  slug: cheniere-energy-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-reference-data-api-openapi.yml
- filename: cheniere-energy-telemetry-api-openapi.yml
  format: yaml
  label: Cheniere Energy Telemetry API
  slug: cheniere-energy-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-telemetry-api-openapi.yml
- filename: cheniere-energy-transactional-reporting-api-openapi.yml
  format: yaml
  label: Cheniere Energy Transactional Reporting API
  slug: cheniere-energy-transactional-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-transactional-reporting-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Cheniere Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cheniere Energy declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Cheniere Energy
provider_slug: cheniere-energy
scheme_count: 0
schemes: []
slug: cheniere-energy-authentication
source_filename: cheniere-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Cheniere Energy\nproviderId: cheniere-energy\ngenerated: '2026-09-06'\nmethod: probed\nsource: >-\n  Anonymous GET requests to https://lngconnectionapi.cheniere.com on 2026-09-06, plus the\n  provider's own client bundle (https://lngconnection.cheniere.com/app.c8746b4fbffdfedeb14b.js),\n  which attaches no Authorization header, no API key and no token acquisition step to any request.\nsummary: >-\n  The Cheniere LNG Connection informational-postings API requires no authentication of any kind.\n  Nine of eleven read endpoints probed anonymously returned HTTP 200 with real posting data; the\n  two failures were server-side 500s, not auth challenges. This is expected and correct: FERC\n  18 CFR 284.13 requires an interstate pipeline to make these postings publicly available without\n  a subscription or a registration barrier.\nschemes: []\nsecurity_requirements: []\nfindings:\n  - id: no-auth-required\n\
  \    detail: >-\n      No securityScheme is declared and none is enforced. There is no signup, no API key, no\n      OAuth flow and no OpenID Connect discovery document on any Cheniere host.\n    evidence:\n      - url: https://lngconnectionapi.cheniere.com/api/Page/GetPages\n        status: 200\n        note: Anonymous request, no headers beyond a User-Agent. Returned the full page tree and TSP list.\n      - url: https://lngconnectionapi.cheniere.com/api/Transactional/GetFirm?tspNo=200&beginDate=2026-09-01&endDate=2026-09-05\n        status: 200\n        note: Anonymous request returned contract-level transactional reporting rows.\n  - id: session-cookie-issued-not-required\n    detail: >-\n      Every response sets an HttpOnly, Secure `LNGConnection` cookie. It is a load-balancer affinity\n      cookie, not a credential — requests sent without it succeed identically.\n    evidence:\n      - url: https://lngconnectionapi.cheniere.com/api/Capacity/GetCycles\n        status: 200\n  - id:\
  \ cors-single-origin\n    detail: >-\n      The API answers a CORS preflight with `Access-Control-Allow-Origin: https://lngconnection.cheniere.com`\n      only. Browser code on any other origin is blocked, while server-side and agent callers are not\n      affected. Worth knowing before planning a browser integration.\n    evidence:\n      - url: https://lngconnectionapi.cheniere.com/api/Capacity/GetCycles\n        status: 200\n        note: OPTIONS preflight with Origin https://lngconnection.cheniere.com returned 200 with a single-origin ACAO header.\n  - id: no-auth-documentation\n    detail: >-\n      Cheniere publishes no developer documentation for this API, so there is no authentication page\n      to cite. The absence of auth is established by probe, not by a provider statement.\n    evidence:\n      - url: https://lngconnectionapi.cheniere.com/swagger/v1/swagger.json\n        status: 404\ntransport:\n  https_required: true\n  tls_version_observed: TLSv1.3\n  server: Microsoft-IIS/10.0\
  \ (ASP.NET Web API 4.0.30319)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/authentication/cheniere-energy-authentication.yml
summary_line: 0 schemes
tags:
- Corpus Christi
- Energy
- Export
- FERC
- Houston
- Informational Postings
- LNG
- Liquefaction
- NAESB
- Natural Gas
- Open Data
- Pipelines
- Regasification
- Sabine Pass
- Texas
---
