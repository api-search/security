---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jsgaiya.cn
  spf: false
hosts:
- host: jsgaiya.cn
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''jsgaiya.cn'''
kind: domain-security
layout: security
method: probed
name: Jsgaiya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jsgaiya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: jsgaiya
provider_slug: jsgaiya
slug: jsgaiya-domain-security
source_filename: jsgaiya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jsgaiya.cn\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''jsgaiya.cn'''\n  hsts: null\ndomains:\n- domain: jsgaiya.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jsgaiya/refs/heads/main/security/jsgaiya-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Environmental Engineering
- Soil Remediation
- Environmental Testing
- Cleantech
- China
- No API Surface
---
