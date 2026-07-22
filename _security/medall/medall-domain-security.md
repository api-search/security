---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medall.org
  spf: true
hosts:
- cert_expires: Sep  9 23:04:21 2026 GMT
  host: medall.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedAll, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MedAll
provider_slug: medall
slug: medall-domain-security
source_filename: medall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medall.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:04:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: medall.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medall/refs/heads/main/security/medall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Education
- Education
- Training
- Events
- Continuing Medical Education
- HealthTech
---
