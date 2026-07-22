---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: truvian.com
  spf: false
hosts:
- host: truvian.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Truvian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truvian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Truvian
provider_slug: truvian
slug: truvian-domain-security
source_filename: truvian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truvian.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: truvian.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truvian/refs/heads/main/security/truvian-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Diagnostics
- Health
- Blood Testing
- Medical Devices
- Point of Care
- Laboratory
---
