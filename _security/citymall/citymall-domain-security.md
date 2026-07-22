---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: citymall.live
  spf: true
hosts:
- cert_expires: Jan 27 08:26:34 2027 GMT
  host: citymall.live
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Citymall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CityMall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CityMall
provider_slug: citymall
slug: citymall-domain-security
source_filename: citymall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citymall.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 08:26:34 2027 GMT\n  hsts: false\ndomains:\n- domain: citymall.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citymall/refs/heads/main/security/citymall-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- E-Commerce
- Social Commerce
- Retail
- Grocery
- India
---
