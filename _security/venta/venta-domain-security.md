---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getventa.ai
  spf: true
hosts:
- cert_expires: Jan 25 05:40:24 2027 GMT
  host: www.getventa.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Venta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Venta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Venta
provider_slug: venta
slug: venta-domain-security
source_filename: venta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getventa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 05:40:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getventa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/venta/security/venta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Outbound
- Manufacturing
- Sales-Automation
- B2B
- Company
---
