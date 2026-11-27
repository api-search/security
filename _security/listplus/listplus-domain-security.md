---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: listplus.ai
  spf: false
hosts:
- cert_expires: Dec 18 02:18:24 2026 GMT
  host: listplus.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ListPlus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ListPlus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ListPlus
provider_slug: listplus
slug: listplus-domain-security
source_filename: listplus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listplus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 02:18:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: listplus.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/listplus/security/listplus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Data Enrichment
- Contact Data
- Artificial Intelligence
- CRM
---
