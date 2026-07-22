---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sh-eco.com.cn
  spf: false
hosts:
- host: sh-eco.com.cn
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Sh Eco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sh-eco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: sh-eco
provider_slug: sh-eco
slug: sh-eco-domain-security
source_filename: sh-eco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sh-eco.com.cn\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: sh-eco.com.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sh-eco/refs/heads/main/security/sh-eco-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Medical Devices
- Materials
- Manufacturing
- Healthcare
- Catheters
- Polymers
- China
---
