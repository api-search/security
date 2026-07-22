---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: docstation.co
  spf: true
hosts:
- cert_expires: Sep 21 06:15:22 2026 GMT
  host: docstation.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docstation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocStation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DocStation
provider_slug: docstation
slug: docstation-domain-security
source_filename: docstation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docstation.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:15:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: docstation.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docstation/refs/heads/main/security/docstation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmacy
- Medical Billing
- Healthcare
- Clinical Services
- Patient Management
- Scheduling
- Insurance Claims
- HIPAA
---
