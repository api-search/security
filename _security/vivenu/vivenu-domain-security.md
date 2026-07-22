---
api_specs:
- filename: vivenu-openapi-original.json
  format: json
  label: vivenu API
  slug: vivenu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivenu/refs/heads/main/openapi/vivenu-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vivenu.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vivenu.dev
  spf: false
hosts:
- cert_expires: Aug 31 06:31:06 2026 GMT
  host: vivenu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 10:32:09 2026 GMT
  host: vivenu.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vivenu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vivenu, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: vivenu
provider_slug: vivenu
slug: vivenu-domain-security
source_filename: vivenu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vivenu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:31:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vivenu.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:32:09 2026 GMT\n  hsts: null\ndomains:\n- domain: vivenu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vivenu.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivenu/refs/heads/main/security/vivenu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Event Ticketing
- Ticketing
- Events
- Payments
- Live Entertainment
- Webhooks
- API-first
---
