---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mint.com
  spf: true
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: www.mint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mint
provider_slug: mint
slug: mint-domain-security
source_filename: mint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mint/refs/heads/main/security/mint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Personal Finance
- Budgeting
- Money Management
- Consumer
- Intuit
---
