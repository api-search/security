---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cybavo.com
  spf: true
hosts:
- host: cybavo.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''cybavo.com'''
kind: domain-security
layout: security
method: probed
name: Cybavo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CYBAVO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CYBAVO
provider_slug: cybavo
slug: cybavo-domain-security
source_filename: cybavo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cybavo.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''cybavo.com'''\n  hsts: null\ndomains:\n- domain: cybavo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybavo/refs/heads/main/security/cybavo-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Digital Asset Security
- Wallet
- Custody
- MPC
- Blockchain
- SDK
---
