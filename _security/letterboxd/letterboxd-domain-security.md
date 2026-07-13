---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Letterboxd API
  slug: letterboxd-api
  spec_type: OpenAPI
  url: https://api-docs.letterboxd.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: letterboxd.com
  spf: true
hosts:
- cert_expires: Aug 19 01:38:44 2026 GMT
  host: letterboxd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 01:38:44 2026 GMT
  host: api.letterboxd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Letterboxd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Letterboxd, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Letterboxd
provider_slug: letterboxd
slug: letterboxd-domain-security
source_filename: letterboxd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letterboxd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 01:38:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.letterboxd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 01:38:44 2026 GMT\n  hsts: null\ndomains:\n- domain: letterboxd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letterboxd/refs/heads/main/security/letterboxd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Film
- Movies
- Social
- Reviews
- Watchlist
- Ratings
- Diary
- Film Festival
- Entertainment
---
