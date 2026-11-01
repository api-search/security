---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vero-software.com
  spf: false
hosts:
- host: www.vero-software.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.vero-so'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vero Software Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vero Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vero Software
provider_slug: vero-software-com
slug: vero-software-com-domain-security
source_filename: vero-software-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vero-software.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.vero-so'\n  hsts: null\ndomains:\n- domain: vero-software.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/vero-software-com/security/vero-software-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
