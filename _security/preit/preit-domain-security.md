---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: preit.com
  spf: true
hosts:
- cert_expires: Aug 16 02:03:59 2026 GMT
  host: www.preit.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Preit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pennsylvania Real Estate Investment Trust (PREIT), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pennsylvania Real Estate Investment Trust (PREIT)
provider_slug: preit
slug: preit-domain-security
source_filename: preit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.preit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 02:03:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: preit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preit/refs/heads/main/security/preit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- REIT
- Shopping Malls
- Retail
- Defunct (Public)
- Chapter 11
- Private Equity
---
