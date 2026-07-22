---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tosummer.cn
  spf: true
hosts:
- cert_expires: Oct  1 08:56:59 2026 GMT
  host: tosummer.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: To Summer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for To Summer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: To Summer
provider_slug: to-summer
slug: to-summer-domain-security
source_filename: to-summer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tosummer.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:56:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tosummer.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/to-summer/refs/heads/main/security/to-summer-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Fragrance
- Beauty
- Lifestyle
- China
---
