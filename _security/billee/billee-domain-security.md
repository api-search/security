---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: billee.ai
  spf: true
hosts:
- cert_expires: Dec 12 09:27:27 2026 GMT
  host: billee.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Billee
provider_slug: billee
slug: billee-domain-security
source_filename: billee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billee.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 09:27:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: billee.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billee/refs/heads/main/security/billee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Utility
- Billing
- Artificial Intelligence
- Multifamily
---
