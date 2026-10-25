---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: premierinvestments.com.au
  spf: true
hosts:
- cert_expires: Dec 13 09:01:49 2026 GMT
  host: premierinvestments.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Premier Investments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Premier Investments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Premier Investments
provider_slug: premier-investments
slug: premier-investments-domain-security
source_filename: premier-investments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: premierinvestments.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 09:01:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: premierinvestments.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/premier-investments/refs/heads/main/security/premier-investments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Investment
- ASX Listed
- Australia
- Importing
- Distribution
---
