---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: keenprint.com
  spf: false
hosts:
- host: keenprint.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''keenprint.c'
kind: domain-security
layout: security
method: probed
name: Keen Print Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keen Print, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Keen Print
provider_slug: keen-print
slug: keen-print-domain-security
source_filename: keen-print-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keenprint.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''keenprint.c'\n  hsts: null\ndomains:\n- domain: keenprint.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keen-print/refs/heads/main/security/keen-print-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
