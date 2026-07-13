---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gruppotim.it
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tim.it
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.gruppotim.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 23:59:59 2026 GMT
  host: www.tim.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.tim.com.br
  hsts: true
  hsts_max_age: 1001
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tim Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TIM, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TIM
provider_slug: tim-com
slug: tim-com-domain-security
source_filename: tim-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gruppotim.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.tim.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.tim.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 1001\ndomains:\n- domain: gruppotim.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tim.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tim-com/refs/heads/main/security/tim-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Telco
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- GSMA
- SIM Swap
- Number Verification
- Know Your Customer
- Identity
- Anti-Fraud
- Italy
- Brazil
- 5G
---
