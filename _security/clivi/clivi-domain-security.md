---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clivi.com.mx
  spf: true
hosts:
- cert_expires: Oct  6 07:59:25 2026 GMT
  host: clivi.com.mx
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clivi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clivi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clivi
provider_slug: clivi
slug: clivi-domain-security
source_filename: clivi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clivi.com.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 07:59:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: clivi.com.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clivi/refs/heads/main/security/clivi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Telemedicine
- Digital Health
- Diabetes
- Obesity
- GLP-1
- Telehealth
- Mexico
---
