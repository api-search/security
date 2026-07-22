---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: verosoftware.com
  spf: true
hosts:
- host: www.verosoftware.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.verosof'
kind: domain-security
layout: security
method: probed
name: Vero Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vero Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vero Software
provider_slug: vero-software
slug: vero-software-domain-security
source_filename: vero-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verosoftware.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.verosof'\n  hsts: null\ndomains:\n- domain: verosoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vero-software/refs/heads/main/security/vero-software-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- CAD
- CAM
- Manufacturing
- Engineering Software
- Machining
- CNC
- Woodworking
- Sheet Metal
---
