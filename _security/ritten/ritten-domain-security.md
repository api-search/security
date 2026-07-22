---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ritten.io
  spf: true
hosts:
- cert_expires: Oct 15 00:40:19 2026 GMT
  host: ritten.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ritten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ritten, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ritten
provider_slug: ritten
slug: ritten-domain-security
source_filename: ritten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ritten.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:40:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ritten.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/security/ritten-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Behavioral Health
- EMR
- EHR
- Healthcare
- Practice Management
- HIPAA
- Revenue Cycle Management
- Clinical Documentation
- Telehealth
---
