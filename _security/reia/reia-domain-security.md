---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reia.com.au
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: www.reia.com.au
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Real Estate Institute of Australia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Real Estate Institute of Australia
provider_slug: reia
slug: reia-domain-security
source_filename: reia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reia.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: reia.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reia/refs/heads/main/security/reia-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Real Estate
- Australia
- Industry Body
- Standards
- Membership
- Property Data
- Housing Affordability
- Research
- Advocacy
- Rentals
- PropTech
---
