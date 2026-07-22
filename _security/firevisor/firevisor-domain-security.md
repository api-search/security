---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firevisor.com
  spf: false
hosts:
- host: firevisor.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''firevisor.c'
kind: domain-security
layout: security
method: probed
name: Firevisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FireVisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FireVisor
provider_slug: firevisor
slug: firevisor-domain-security
source_filename: firevisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firevisor.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''firevisor.c'\n  hsts: null\ndomains:\n- domain: firevisor.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firevisor/refs/heads/main/security/firevisor-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Manufacturing
- Analytics
- Artificial Intelligence
- Industrial Automation
- Defect Detection
- Machine Learning
---
