---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aggredyne.com
  spf: true
hosts:
- host: www.aggredyne.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aggredyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AggreDyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AggreDyne
provider_slug: aggredyne
slug: aggredyne-domain-security
source_filename: aggredyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aggredyne.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: aggredyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aggredyne/refs/heads/main/security/aggredyne-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Medical Devices
- Diagnostics
- In Vitro Diagnostics
- Healthcare
- Hematology
- Platelet Function Testing
- Laboratory
- Manufacturing
---
