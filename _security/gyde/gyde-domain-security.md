---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gydehealth.ai
  spf: true
hosts:
- cert_expires: Aug 29 14:17:22 2026 GMT
  host: www.gydehealth.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gyde Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gyde, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gyde
provider_slug: gyde
slug: gyde-domain-security
source_filename: gyde-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gydehealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 14:17:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gydehealth.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gyde/refs/heads/main/security/gyde-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Health Insurance
- Artificial Intelligence
- Brokerage
- AI Assistant
- Austin
---
