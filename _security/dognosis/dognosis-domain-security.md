---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dognosis.tech
  spf: true
hosts:
- cert_expires: Aug 25 01:33:49 2026 GMT
  host: dognosis.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dognosis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dognosis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dognosis
provider_slug: dognosis
slug: dognosis-domain-security
source_filename: dognosis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dognosis.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 01:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dognosis.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dognosis/refs/heads/main/security/dognosis-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Cancer Detection
- Breath Analysis
- Olfaction AI
- Deeptech
---
