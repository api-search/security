---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 100.me
  spf: true
hosts:
- cert_expires: Oct 29 01:31:30 2026 GMT
  host: www.100.me
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dingdong Maicai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dingdong Maicai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dingdong Maicai
provider_slug: dingdong-maicai
slug: dingdong-maicai-domain-security
source_filename: dingdong-maicai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.100.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 01:31:30 2026 GMT\n  hsts: null\ndomains:\n- domain: 100.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dingdong-maicai/refs/heads/main/security/dingdong-maicai-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Consumer
- Grocery
- E-commerce
- Food Delivery
- Retail
- Fresh Produce
- China
---
