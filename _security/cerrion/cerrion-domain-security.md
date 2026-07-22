---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cerrion.com
  spf: true
hosts:
- cert_expires: Sep 26 10:04:36 2026 GMT
  host: www.cerrion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerrion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerrion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cerrion
provider_slug: cerrion
slug: cerrion-domain-security
source_filename: cerrion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cerrion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:04:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cerrion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerrion/refs/heads/main/security/cerrion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Computer Vision
- Manufacturing
- Video Analytics
- Industrial Automation
- Quality Assurance
- Safety Monitoring
---
