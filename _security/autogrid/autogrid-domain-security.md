---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: auto-grid.com
  spf: true
hosts:
- host: auto-grid.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Autogrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoGrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AutoGrid
provider_slug: autogrid
slug: autogrid-domain-security
source_filename: autogrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auto-grid.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: auto-grid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autogrid/refs/heads/main/security/autogrid-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Grid
- DERMS
- Distributed Energy Resources
- Virtual Power Plant
- Demand Response
- Acquired
- OpenADR
- IEEE 2030.5
- Smart Grid
- Conformance
---
