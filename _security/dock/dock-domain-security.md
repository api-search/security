---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dock.tech
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caradhras.io
  spf: true
hosts:
- cert_expires: Sep 14 04:47:08 2026 GMT
  host: dock.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:40:49 2026 GMT
  host: developers.dock.tech
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api.caradhras.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dock, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dock
provider_slug: dock
slug: dock-domain-security
source_filename: dock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dock.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:47:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.dock.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:40:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.caradhras.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dock.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: caradhras.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dock/refs/heads/main/security/dock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Payments
- Cards
- Card Issuing
- Banking as a Service
- Financial-Services
- Fintech
- Pix
- Digital Accounts
- Acquiring
- Anti-Fraud
- Embedded Finance
- Brazil
- Latin America
---
