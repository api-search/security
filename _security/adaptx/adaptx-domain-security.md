---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adaptx.com
  spf: true
hosts:
- cert_expires: Nov 26 17:24:28 2026 GMT
  host: www.adaptx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adaptx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdaptX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AdaptX
provider_slug: adaptx
slug: adaptx-domain-security
source_filename: adaptx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adaptx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 17:24:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adaptx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptx/refs/heads/main/security/adaptx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Healthcare Analytics
- Clinical Data
- Electronic Medical Records
- Hospital Operations
- Quality Improvement
- Business Intelligence
- SaaS
- Seattle
---
