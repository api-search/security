---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: houseeazy.com
  spf: true
hosts:
- cert_expires: Aug 20 06:40:56 2026 GMT
  host: houseeazy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Houseeazy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HouseEazy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HouseEazy
provider_slug: houseeazy
slug: houseeazy-domain-security
source_filename: houseeazy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: houseeazy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:40:56 2026 GMT\n  hsts: false\ndomains:\n- domain: houseeazy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/houseeazy/refs/heads/main/security/houseeazy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Real Estate
- PropTech
- Property
- Resale
- India
- Housing
---
