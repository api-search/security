---
api_specs:
- filename: fred-categories-api-openapi.yml
  format: yaml
  label: FRED Categories API
  slug: fred-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-categories-api-openapi.yml
- filename: fred-observations-api-openapi.yml
  format: yaml
  label: FRED Observations API
  slug: fred-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-observations-api-openapi.yml
- filename: fred-regional-data-api-openapi.yml
  format: yaml
  label: FRED Regional Data API
  slug: fred-regional-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-regional-data-api-openapi.yml
- filename: fred-releases-api-openapi.yml
  format: yaml
  label: FRED Releases API
  slug: fred-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-releases-api-openapi.yml
- filename: fred-series-api-openapi.yml
  format: yaml
  label: FRED Series API
  slug: fred-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-series-api-openapi.yml
- filename: fred-series-data-api-openapi.yml
  format: yaml
  label: FRED Series Data API
  slug: fred-series-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-series-data-api-openapi.yml
- filename: fred-series-group-api-openapi.yml
  format: yaml
  label: FRED Series Group API
  slug: fred-series-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-series-group-api-openapi.yml
- filename: fred-shapes-api-openapi.yml
  format: yaml
  label: FRED Shapes API
  slug: fred-shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-shapes-api-openapi.yml
- filename: fred-sources-api-openapi.yml
  format: yaml
  label: FRED Sources API
  slug: fred-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-sources-api-openapi.yml
- filename: fred-tags-api-openapi.yml
  format: yaml
  label: FRED Tags API
  slug: fred-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stlouisfed.org
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: fred.stlouisfed.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.stlouisfed.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fred Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FRED, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FRED
provider_slug: fred
slug: fred-domain-security
source_filename: fred-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fred.stlouisfed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\n- host: api.stlouisfed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: stlouisfed.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/security/fred-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Government
- Economic Data
- Federal Reserve
- Time Series
- Open Data
- Public APIs
---
