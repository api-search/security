---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ohmysynt.io
  spf: true
hosts:
- host: ohmysynt.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ohmysynt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OHMYSYNT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OHMYSYNT
provider_slug: ohmysynt
slug: ohmysynt-domain-security
source_filename: ohmysynt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ohmysynt.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ohmysynt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ohmysynt/refs/heads/main/security/ohmysynt-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
