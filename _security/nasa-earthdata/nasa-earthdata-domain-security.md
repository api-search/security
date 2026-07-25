---
api_specs:
- filename: nasa-earthdata-capabilities-api-openapi.yml
  format: yaml
  label: NASA Earthdata Capabilities API
  slug: nasa-earthdata-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/openapi/nasa-earthdata-capabilities-api-openapi.yml
- filename: nasa-earthdata-coverage-api-openapi.yml
  format: yaml
  label: NASA Earthdata Coverage API
  slug: nasa-earthdata-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/openapi/nasa-earthdata-coverage-api-openapi.yml
- filename: nasa-earthdata-openapi-api-openapi.yml
  format: yaml
  label: NASA Earthdata OpenAPI API
  slug: nasa-earthdata-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/openapi/nasa-earthdata-openapi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nasa.gov
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: www.earthdata.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: cmr.earthdata.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: urs.earthdata.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nasa Earthdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NASA Earthdata, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NASA Earthdata
provider_slug: nasa-earthdata
slug: nasa-earthdata-domain-security
source_filename: nasa-earthdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.earthdata.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cmr.earthdata.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: urs.earthdata.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/security/nasa-earthdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Earth Observation
- Satellite Data
- Climate Data
- Remote Sensing
- Geospatial
- NASA
- Science Data
---
