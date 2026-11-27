---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: longbook.app
  spf: true
hosts:
- cert_expires: Dec 30 21:41:50 2026 GMT
  host: longbook.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Longbook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Longbook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Longbook
provider_slug: longbook-app
slug: longbook-app-domain-security
source_filename: longbook-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: longbook.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 21:41:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: longbook.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/longbook-app/security/longbook-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bank Statements
- financial memory
- Personal Finance
- iPhone App
- macOS app
---
