---
api_specs:
- filename: lettance-com-openapi.json
  format: json
  label: Lettance Public API
  slug: lettance-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lettance-com/openapi/lettance-com-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lettance.com
  spf: false
hosts:
- cert_expires: Jan 12 10:17:16 2027 GMT
  host: lettance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lettance Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lettance-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: lettance-com
provider_slug: lettance-com
slug: lettance-com-domain-security
source_filename: lettance-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lettance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 10:17:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lettance.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lettance-com/security/lettance-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Leasing
- Subscription
- API
- Automation
---
