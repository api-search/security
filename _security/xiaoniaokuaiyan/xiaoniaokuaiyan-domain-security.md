---
description: ''
domains:
- caa:
  - www.xiaoniao99.com.
  dmarc: false
  dnssec: false
  domain: xiaoniaokuaiyan.com
  spf: false
hosts:
- host: xiaoniaokuaiyan.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''xiaoniaokua'
kind: domain-security
layout: security
method: probed
name: Xiaoniaokuaiyan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xiaoniaokuaiyan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: xiaoniaokuaiyan
provider_slug: xiaoniaokuaiyan
slug: xiaoniaokuaiyan-domain-security
source_filename: xiaoniaokuaiyan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xiaoniaokuaiyan.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''xiaoniaokua'\n  hsts: null\ndomains:\n- domain: xiaoniaokuaiyan.com\n  dnssec: false\n  caa:\n  - www.xiaoniao99.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaoniaokuaiyan/refs/heads/main/security/xiaoniaokuaiyan-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Healthcare
- Health
- Medical Testing
- Diagnostics
- Home Health
- China
- Internet Hospital
---
