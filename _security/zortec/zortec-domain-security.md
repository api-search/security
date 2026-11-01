---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zortec.com
  spf: true
hosts:
- host: zortec.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''zortec.com'''
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zortec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zortec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zortec
provider_slug: zortec
slug: zortec-domain-security
source_filename: zortec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zortec.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''zortec.com'''\n  hsts: null\ndomains:\n- domain: zortec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/zortec/security/zortec-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Integration
- Modernization
- Enterprise
- Software
---
