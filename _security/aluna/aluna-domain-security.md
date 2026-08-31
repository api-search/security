---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alunacare.com
  spf: true
hosts:
- cert_expires: Aug 29 13:57:03 2026 GMT
  host: alunacare.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aluna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aluna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aluna
provider_slug: aluna
slug: aluna-domain-security
source_filename: aluna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alunacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 13:57:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: alunacare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aluna/refs/heads/main/security/aluna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthtech
- Respiratory
- Spirometry
- Remote Patient Monitoring
- Digital Health
- Medical Device
- Asthma
- COPD
---
