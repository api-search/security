---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: baicaiche.com
  spf: false
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: www.baicaiche.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Baicai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baicai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Baicai
provider_slug: baicai
slug: baicai-domain-security
source_filename: baicai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baicaiche.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: baicaiche.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baicai/refs/heads/main/security/baicai-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Automotive
- Used Cars
- Marketplace
- E-Commerce
- Consumer
- China
- Ribbit Capital
---
