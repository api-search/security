---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: barn2door.com
  spf: true
hosts:
- cert_expires: Sep 16 02:18:46 2026 GMT
  host: www.barn2door.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barn2Door Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barn2Door, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Barn2Door
provider_slug: barn2door
slug: barn2door-domain-security
source_filename: barn2door-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.barn2door.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:18:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: barn2door.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barn2door/refs/heads/main/security/barn2door-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Food
- E-Commerce
- Farm Management
- Local Food
- Payments
- Logistics
- SaaS
---
