---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: effa.one
  spf: true
hosts:
- host: effa.one
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''effa.one''. '
kind: domain-security
layout: security
method: probed
name: Effa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Effa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Effa
provider_slug: effa
slug: effa-domain-security
source_filename: effa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: effa.one\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''effa.one''. '\n  hsts: null\ndomains:\n- domain: effa.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/effa/refs/heads/main/security/effa-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer Goods
- Sustainability
- Personal Care
- Hospitality
- Manufacturing
---
