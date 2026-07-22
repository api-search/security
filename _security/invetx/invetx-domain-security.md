---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: invetx.com
  spf: true
hosts:
- host: invetx.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''invetx.com'''
kind: domain-security
layout: security
method: probed
name: Invetx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invetx *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Invetx *
provider_slug: invetx
slug: invetx-domain-security
source_filename: invetx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invetx.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''invetx.com'''\n  hsts: null\ndomains:\n- domain: invetx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invetx/refs/heads/main/security/invetx-domain-security.yml
summary_line: DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Animal Health
- Veterinary
- Monoclonal Antibodies
- Therapeutics
- Acquired
---
