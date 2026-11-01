---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: netbrainis.co.za
  spf: true
hosts:
- host: netbrainis.co.za
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netbrainis Co Za Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for netbrainis-co-za, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: netbrainis-co-za
provider_slug: netbrainis-co-za
slug: netbrainis-co-za-domain-security
source_filename: netbrainis-co-za-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netbrainis.co.za\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: netbrainis.co.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/netbrainis-co-za/security/netbrainis-co-za-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
