---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autochilango.com
  spf: true
hosts:
- host: autochilango.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''autochilang'
kind: domain-security
layout: security
method: probed
name: Autochilango Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoChilango, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AutoChilango
provider_slug: autochilango
slug: autochilango-domain-security
source_filename: autochilango-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autochilango.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''autochilang'\n  hsts: null\ndomains:\n- domain: autochilango.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autochilango/refs/heads/main/security/autochilango-domain-security.yml
summary_line: DMARC
tags:
- Company
- Automotive
- Mobile App
- Mexico
- Mexico City
- Drivers
- Consumer
- Transportation
---
