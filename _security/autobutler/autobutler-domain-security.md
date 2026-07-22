---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: autobutler.dk
  spf: true
hosts:
- cert_expires: Sep  5 21:59:08 2026 GMT
  host: www.autobutler.dk
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autobutler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autobutler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Autobutler
provider_slug: autobutler
slug: autobutler-domain-security
source_filename: autobutler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autobutler.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 21:59:08 2026 GMT\n  hsts: true\n  hsts_max_age: 600\ndomains:\n- domain: autobutler.dk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autobutler/refs/heads/main/security/autobutler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Automotive
- Marketplace
- Car Repair
- Price Comparison
- Denmark
---
