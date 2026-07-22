---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tisenc.com
  spf: true
hosts:
- host: tisenc.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Tisenc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tisenc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: tisenc
provider_slug: tisenc
slug: tisenc-domain-security
source_filename: tisenc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tisenc.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: tisenc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tisenc/refs/heads/main/security/tisenc-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Medical Devices
- In-Vitro Diagnostics
- Diagnostics
- Chemiluminescence Immunoassay
- Point-of-Care Testing
- Healthcare
- China
---
