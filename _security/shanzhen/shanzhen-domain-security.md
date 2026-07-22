---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shanzhen.me
  spf: false
hosts:
- host: shanzhen.me
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Shanzhen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shanzhen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: shanzhen
provider_slug: shanzhen
slug: shanzhen-domain-security
source_filename: shanzhen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shanzhen.me\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: shanzhen.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shanzhen/refs/heads/main/security/shanzhen-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
