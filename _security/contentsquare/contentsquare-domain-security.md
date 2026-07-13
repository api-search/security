---
api_specs:
- filename: contentsquare-openapi.yml
  format: yaml
  label: Contentsquare Data Export API
  slug: data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentsquare/refs/heads/main/openapi/contentsquare-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: contentsquare.com
  spf: true
hosts:
- cert_expires: Aug 20 17:00:09 2026 GMT
  host: contentsquare.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 19:00:08 2026 GMT
  host: docs.contentsquare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 13:35:22 2026 GMT
  host: api.eu-west-1.production.contentsquare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contentsquare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contentsquare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Contentsquare
provider_slug: contentsquare
slug: contentsquare-domain-security
source_filename: contentsquare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contentsquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:00:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.contentsquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:00:08 2026 GMT\n  hsts: false\n- host: api.eu-west-1.production.contentsquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 13:35:22 2026 GMT\n  hsts: null\ndomains:\n- domain: contentsquare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentsquare/refs/heads/main/security/contentsquare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Digital Experience Analytics
- Product Analytics
- Session Replay
- Heatmaps
- Customer Experience
- Conversion Optimization
- User Behavior
---
