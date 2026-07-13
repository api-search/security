---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: mocky.io
  spf: false
hosts:
- host: designer.mocky.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Mocky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mocky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Mocky
provider_slug: mocky
slug: mocky-domain-security
source_filename: mocky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: designer.mocky.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: mocky.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mocky/refs/heads/main/security/mocky-domain-security.yml
summary_line: DNSSEC
tags:
- Development
- Public APIs
---
