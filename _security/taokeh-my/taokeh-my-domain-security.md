---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: taokeh.my
  spf: true
hosts:
- cert_expires: Jan  9 13:46:39 2027 GMT
  host: taokeh.my
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taokeh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taokeh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Taokeh
provider_slug: taokeh-my
slug: taokeh-my-domain-security
source_filename: taokeh-my-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taokeh.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 13:46:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taokeh.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/taokeh-my/security/taokeh-my-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Payroll
- e‑Invoice
- SME Software
- Marketplace Integration
---
