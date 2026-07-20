---
api_specs:
- filename: distru-openapi.yml
  format: yaml
  label: Distru Public API
  slug: distru-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distru/refs/heads/main/openapi/distru-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: distru.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: distru.dev
  spf: false
hosts:
- cert_expires: Sep 11 04:44:53 2026 GMT
  host: www.distru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 12:25:26 2026 GMT
  host: apidocs.distru.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 21:27:39 2026 GMT
  host: app.distru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Distru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Distru, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Distru
provider_slug: distru
slug: distru-domain-security
source_filename: distru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.distru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:44:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.distru.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 12:25:26 2026 GMT\n  hsts: false\n- host: app.distru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:27:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: distru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: distru.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distru/refs/heads/main/security/distru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cannabis
- ERP
- Seed-to-Sale
- Inventory
- Compliance
- Distribution
- Manufacturing
- Wholesale
- Metrc
---
