---
api_specs:
- filename: bureau-of-transportation-statistics-openapi.yml
  format: yaml
  label: BTS Open Data SODA API
  slug: bts-open-data-soda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-transportation-statistics/refs/heads/main/openapi/bureau-of-transportation-statistics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bts.gov
  spf: true
hosts:
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: www.bts.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 18:23:49 2026 GMT
  host: data.bts.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.transtats.bts.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bureau Of Transportation Statistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Transportation Statistics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Transportation Statistics
provider_slug: bureau-of-transportation-statistics
slug: bureau-of-transportation-statistics-domain-security
source_filename: bureau-of-transportation-statistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: null\n- host: data.bts.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 18:23:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.transtats.bts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bts.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-transportation-statistics/refs/heads/main/security/bureau-of-transportation-statistics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Statistics
- Transportation
- Aviation
- Freight
- Open Data
---
