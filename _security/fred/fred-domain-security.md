---
api_specs:
- filename: fred-openapi.yml
  format: yaml
  label: FRED API
  slug: fred-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-openapi.yml
- filename: fred-geofred-openapi.yml
  format: yaml
  label: FRED Maps API (GeoFRED)
  slug: fred-maps-api-geofred
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-geofred-openapi.yml
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
