---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: icf.com
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.icf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Icf International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ICF (ICF International), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ICF (ICF International)
provider_slug: icf-international
slug: icf-international-domain-security
source_filename: icf-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icf.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: icf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icf-international/refs/heads/main/security/icf-international-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Federal Consulting
- Digital Modernization
- Energy
- Environment
- Disaster Management
- Federal Health
- Public Sector IT
- AI Consulting
---
