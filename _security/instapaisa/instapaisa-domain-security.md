---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: instapaisa.com
  spf: true
hosts:
- host: instapaisa.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''instapaisa.'
kind: domain-security
layout: security
method: probed
name: Instapaisa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InstaPaisa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: InstaPaisa
provider_slug: instapaisa
slug: instapaisa-domain-security
source_filename: instapaisa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instapaisa.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''instapaisa.'\n  hsts: null\ndomains:\n- domain: instapaisa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instapaisa/refs/heads/main/security/instapaisa-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Fintech
- Lending
- Personal Finance
- Payments
- India
- 500 Global
- Acquired
---
