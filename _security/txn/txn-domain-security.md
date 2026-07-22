---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: txn.com
  spf: false
hosts:
- host: txn.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate in certificate chain (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Txn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TXN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TXN
provider_slug: txn
slug: txn-domain-security
source_filename: txn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: txn.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    in certificate chain (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: txn.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/txn/refs/heads/main/security/txn-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Analytics
- Consumer Spending
- Market Research
- Competitive Intelligence
- Surveys
---
