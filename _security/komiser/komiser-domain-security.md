---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: komiser.io
  spf: false
hosts:
- host: www.komiser.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Komiser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Komiser, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Komiser
provider_slug: komiser
slug: komiser-domain-security
source_filename: komiser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.komiser.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: komiser.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komiser/refs/heads/main/security/komiser-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Cloud Cost
- FinOps
- Governance
- Multi-Cloud
- Open Source
---
