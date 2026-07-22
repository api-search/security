---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: finern.com
  spf: true
hosts:
- host: finern.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''finern.com'''
kind: domain-security
layout: security
method: probed
name: Finern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for finern, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: finern
provider_slug: finern
slug: finern-domain-security
source_filename: finern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finern.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''finern.com'''\n  hsts: null\ndomains:\n- domain: finern.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finern/refs/heads/main/security/finern-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Industrial Automation
- Manufacturing
- Automation
- Intelligent Measurement
- Robotics
- Automotive
- Electronics
- New Energy
---
