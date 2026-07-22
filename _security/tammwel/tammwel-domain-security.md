---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tamawal.sa
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: tamawal.sa
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tammwel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tammwel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tammwel
provider_slug: tammwel
slug: tammwel-domain-security
source_filename: tammwel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tamawal.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tamawal.sa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tammwel/refs/heads/main/security/tammwel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- Personal Finance
- Saudi Arabia
- Islamic Finance
- Comparison Platform
---
