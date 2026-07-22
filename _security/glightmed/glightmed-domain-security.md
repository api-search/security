---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: glightmed.com
  spf: true
hosts:
- host: glightmed.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''glightmed.c'
kind: domain-security
layout: security
method: probed
name: Glightmed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for glightmed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: glightmed
provider_slug: glightmed
slug: glightmed-domain-security
source_filename: glightmed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glightmed.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''glightmed.c'\n  hsts: null\ndomains:\n- domain: glightmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glightmed/refs/heads/main/security/glightmed-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
