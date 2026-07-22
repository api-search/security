---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trendyent.com
  spf: true
hosts:
- host: trendyent.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''trendyent.c'
kind: domain-security
layout: security
method: probed
name: Trendy Entertainment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trendy Entertainment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Trendy Entertainment
provider_slug: trendy-entertainment
slug: trendy-entertainment-domain-security
source_filename: trendy-entertainment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trendyent.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''trendyent.c'\n  hsts: null\ndomains:\n- domain: trendyent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trendy-entertainment/refs/heads/main/security/trendy-entertainment-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Gaming
- Video Games
- Game Studio
- Tower Defense
- Dungeon Defenders
- Entertainment
---
