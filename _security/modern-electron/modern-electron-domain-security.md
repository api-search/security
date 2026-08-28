---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modernhydrogen.com
  spf: true
hosts:
- host: modernhydrogen.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''modernhydro'
kind: domain-security
layout: security
method: probed
name: Modern Electron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modern Electron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Modern Electron
provider_slug: modern-electron
slug: modern-electron-domain-security
source_filename: modern-electron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modernhydrogen.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''modernhydro'\n  hsts: null\ndomains:\n- domain: modernhydrogen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modern-electron/refs/heads/main/security/modern-electron-domain-security.yml
summary_line: DMARC
tags:
- Company
- Energy
- Hydrogen
- Clean Energy
- Hardware
- Manufacturing
- Climate Tech
- Thermionics
---
