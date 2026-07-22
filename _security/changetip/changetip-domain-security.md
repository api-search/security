---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: changetip.com
  spf: false
hosts:
- host: changetip.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''changetip.c'
kind: domain-security
layout: security
method: probed
name: Changetip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChangeTip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ChangeTip
provider_slug: changetip
slug: changetip-domain-security
source_filename: changetip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: changetip.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''changetip.c'\n  hsts: null\ndomains:\n- domain: changetip.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/changetip/refs/heads/main/security/changetip-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Bitcoin
- Cryptocurrency
- Micropayments
- Payments
- Tipping
- Social Media
- Wallet
- Defunct
---
