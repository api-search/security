---
api_specs:
- filename: regal-cinema-openapi.yml
  format: yaml
  label: Regal Cinema API
  slug: regal-cinema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-entertainment-group/refs/heads/main/openapi/regal-cinema-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: regmovies.com
  spf: true
hosts:
- cert_expires: Aug 14 19:56:51 2026 GMT
  host: www.regmovies.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 19:56:51 2026 GMT
  host: developer.regmovies.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.regmovies.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regal Entertainment Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for regal-entertainment-group, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: regal-entertainment-group
provider_slug: regal-entertainment-group
slug: regal-entertainment-group-domain-security
source_filename: regal-entertainment-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regmovies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 19:56:51 2026 GMT\n  hsts: null\n- host: developer.regmovies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 19:56:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.regmovies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: regmovies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-entertainment-group/refs/heads/main/security/regal-entertainment-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cinema
- Entertainment
- Movies
- Ticketing
- Loyalty
- Theatre
- Fortune 500
---
