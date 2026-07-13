---
api_specs:
- filename: stats-perform-stats-api-openapi.yml
  format: yaml
  label: STATS API
  slug: stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stats-perform/refs/heads/main/openapi/stats-perform-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stats.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: developer.stats.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 20:14:04 2026 GMT
  host: api.stats.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stats Perform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stats Perform, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Stats Perform
provider_slug: stats-perform
slug: stats-perform-domain-security
source_filename: stats-perform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.stats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\n- host: api.stats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 20:14:04 2026 GMT\n  hsts: null\ndomains:\n- domain: stats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stats-perform/refs/heads/main/security/stats-perform-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports
- Sports Data
- Football
- Baseball
- Basketball
- Hockey
- Soccer
- Golf
- Tennis
- Live Scores
- Statistics
- Sports Analytics
---
