---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: apidash.dev
  spf: true
hosts:
- cert_expires: Sep  1 08:24:36 2026 GMT
  host: apidash.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Dash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Dash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: API Dash
provider_slug: api-dash
slug: api-dash-domain-security
source_filename: api-dash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidash.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 08:24:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: apidash.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/security/api-dash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- API Client
- Open Source
- Flutter
- Desktop
- Mobile
---
