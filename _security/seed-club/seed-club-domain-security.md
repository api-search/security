---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: seedclub.xyz
  spf: false
hosts:
- host: seedclub.xyz
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Seed Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seed Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Seed Club
provider_slug: seed-club
slug: seed-club-domain-security
source_filename: seed-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seedclub.xyz\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: seedclub.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seed-club/refs/heads/main/security/seed-club-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Crypto Web3
- Accelerator
- Venture Capital
- Consumer Crypto
- Web3 Communities
- Creator Economy
---
