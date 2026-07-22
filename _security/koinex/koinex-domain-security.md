---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: koinex.in
  spf: false
hosts:
- host: koinex.in
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Koinex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koinex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Koinex
provider_slug: koinex
slug: koinex-domain-security
source_filename: koinex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koinex.in\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: koinex.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koinex/refs/heads/main/security/koinex-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Crypto
- Cryptocurrency Exchange
- Digital Assets
- Trading
- India
- Fintech
- Defunct
---
