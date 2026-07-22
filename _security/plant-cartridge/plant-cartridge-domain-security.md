---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: plantcartridge.com
  spf: true
hosts:
- host: plantcartridge.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Plant Cartridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plant Cartridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Plant Cartridge
provider_slug: plant-cartridge
slug: plant-cartridge-domain-security
source_filename: plant-cartridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plantcartridge.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: plantcartridge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plant-cartridge/refs/heads/main/security/plant-cartridge-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Agriculture
- AgTech
- Vertical Farming
- Indoor Farming
- Sustainability
- Growing Systems
- Food
---
