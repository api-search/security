---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: metaphorpsum.com
  spf: false
hosts:
- host: metaphorpsum.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''metaphorpsu'
kind: domain-security
layout: security
method: probed
name: Metaphorsum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metaphorsum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Metaphorsum
provider_slug: metaphorsum
slug: metaphorsum-domain-security
source_filename: metaphorsum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metaphorpsum.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''metaphorpsu'\n  hsts: null\ndomains:\n- domain: metaphorpsum.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metaphorsum/refs/heads/main/security/metaphorsum-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Test Data
- Public APIs
---
