---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: divide.com
  spf: true
hosts:
- host: divide.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''divide.com'''
kind: domain-security
layout: security
method: probed
name: Divide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Divide *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Divide *
provider_slug: divide
slug: divide-domain-security
source_filename: divide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: divide.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''divide.com'''\n  hsts: null\ndomains:\n- domain: divide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/divide/refs/heads/main/security/divide-domain-security.yml
summary_line: DMARC
tags:
- Company
- Enterprise
- Mobile
- BYOD
- Mobile Device Management
- Security
- Acquired
---
