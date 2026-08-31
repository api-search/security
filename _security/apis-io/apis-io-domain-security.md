---
api_specs:
- filename: apis-io-apis-api-openapi.yml
  format: yaml
  label: APIs.io APIs API
  slug: apis-io-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-apis-api-openapi.yml
- filename: apis-io-areas-api-openapi.yml
  format: yaml
  label: APIs.io Areas API
  slug: apis-io-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-areas-api-openapi.yml
- filename: apis-io-artifact-types-api-openapi.yml
  format: yaml
  label: APIs.io Artifact Types API
  slug: apis-io-artifact-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-artifact-types-api-openapi.yml
- filename: apis-io-industries-api-openapi.yml
  format: yaml
  label: APIs.io Industries API
  slug: apis-io-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-industries-api-openapi.yml
- filename: apis-io-insights-api-openapi.yml
  format: yaml
  label: APIs.io Insights API
  slug: apis-io-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-insights-api-openapi.yml
- filename: apis-io-providers-api-openapi.yml
  format: yaml
  label: APIs.io Providers API
  slug: apis-io-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-providers-api-openapi.yml
- filename: apis-io-ratings-api-openapi.yml
  format: yaml
  label: APIs.io Ratings API
  slug: apis-io-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-ratings-api-openapi.yml
- filename: apis-io-regions-api-openapi.yml
  format: yaml
  label: APIs.io Regions API
  slug: apis-io-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-regions-api-openapi.yml
- filename: apis-io-search-api-openapi.yml
  format: yaml
  label: APIs.io Search API
  slug: apis-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-search-api-openapi.yml
- filename: apis-io-synthesis-api-openapi.yml
  format: yaml
  label: APIs.io Synthesis API
  slug: apis-io-synthesis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-synthesis-api-openapi.yml
- filename: apis-io-tags-api-openapi.yml
  format: yaml
  label: APIs.io Tags API
  slug: apis-io-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-tags-api-openapi.yml
- filename: apis-io-v1-cohorts-openapi.yml
  format: yaml
  label: APIs.io Cohorts API
  slug: apis-io-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-v1-cohorts-openapi.yml
- filename: apis-io-v1-editorial-openapi.yml
  format: yaml
  label: APIs.io Editorial API
  slug: apis-io-editorial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-v1-editorial-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apis.io
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: apis.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apis Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIs.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: APIs.io
provider_slug: apis-io
slug: apis-io-domain-security
source_filename: apis-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\n# 2026-08-21: dropped the search-api.apis.io entry. The probe was honest -- the\n# host had no DNS record -- but listing it under `hosts` asserts a host we\n# operate. It only appeared here because 11 OpenAPI documents declared it as\n# their server; those now declare https://apis.io/api/v1, which resolves.\nhosts:\n- host: apis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: apis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/security/apis-io-domain-security.yml
summary_line: TLSv1.3
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engines
- API Catalog
- Agent Discovery
- MCP
- Agent Skills
- OpenAPI
- API Governance
---
