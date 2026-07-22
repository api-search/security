---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: extremeprogramming.org
  spf: false
hosts:
- host: www.extremeprogramming.org
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.extreme'
kind: domain-security
layout: security
method: probed
name: Extreme Programming Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extreme Programming, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Extreme Programming
provider_slug: extreme-programming
slug: extreme-programming-domain-security
source_filename: extreme-programming-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.extremeprogramming.org\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.extreme'\n  hsts: null\ndomains:\n- domain: extremeprogramming.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extreme-programming/refs/heads/main/security/extreme-programming-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Agile
- Extreme Programming
- Software Development
- XP
---
