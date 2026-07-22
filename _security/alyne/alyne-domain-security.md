---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alyne.com
  spf: true
hosts:
- cert_expires: Aug 20 08:43:40 2026 GMT
  host: alyne.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alyne
provider_slug: alyne
slug: alyne-domain-security
source_filename: alyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 08:43:40 2026 GMT\n  hsts: false\ndomains:\n- domain: alyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alyne/refs/heads/main/security/alyne-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Governance Risk and Compliance
- GRC
- Risk Management
- Compliance
- Security
- Cybersecurity
- Enterprise Software
- SaaS
---
