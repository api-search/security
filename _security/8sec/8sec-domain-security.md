---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 8sec.games
  spf: true
hosts:
- host: 8sec.games
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''8sec.games'''
kind: domain-security
layout: security
method: probed
name: 8Sec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 8sec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 8sec
provider_slug: 8sec
slug: 8sec-domain-security
source_filename: 8sec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 8sec.games\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''8sec.games'''\n  hsts: null\ndomains:\n- domain: 8sec.games\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/8sec/refs/heads/main/security/8sec-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Games
- Mobile Games
- Game Studio
- Hyper-Casual
- Gaming
- France
---
