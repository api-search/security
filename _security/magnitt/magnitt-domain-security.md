---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: magnitt.com
  spf: true
hosts:
- cert_expires: Sep 27 13:09:30 2026 GMT
  host: magnitt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magnitt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MAGNiTT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MAGNiTT
provider_slug: magnitt
slug: magnitt-domain-security
source_filename: magnitt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magnitt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:09:30 2026 GMT\n  hsts: null\ndomains:\n- domain: magnitt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magnitt/refs/heads/main/security/magnitt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Venture Capital
- Startups
- Data Platform
- Market Research
- Investors
- MENA
- Emerging Markets
- Analytics
---
