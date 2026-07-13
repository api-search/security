---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mgnet.me
  spf: true
hosts:
- host: mgnet.me
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Mgnet Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mgnet.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mgnet.me
provider_slug: mgnet-me
slug: mgnet-me-domain-security
source_filename: mgnet-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mgnet.me\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: mgnet.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mgnet-me/refs/heads/main/security/mgnet-me-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- URL Shorteners
- Public APIs
---
