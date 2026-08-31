---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: swiftmile.com
  spf: true
hosts:
- host: swiftmile.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''swiftmile.c'
kind: domain-security
layout: security
method: probed
name: Swiftmile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swiftmile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Swiftmile
provider_slug: swiftmile
slug: swiftmile-domain-security
source_filename: swiftmile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swiftmile.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''swiftmile.c'\n  hsts: null\ndomains:\n- domain: swiftmile.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftmile/refs/heads/main/security/swiftmile-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Micromobility
- Electric Vehicle Charging
- Transportation
- Internet of Things
- Hardware
- Smart Cities
- Fleet Management
---
