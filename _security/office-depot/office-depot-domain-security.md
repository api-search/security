---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: office-depot.com
  spf: true
hosts:
- host: www.office-depot.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Office Depot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Office Depot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Office Depot
provider_slug: office-depot
slug: office-depot-domain-security
source_filename: office-depot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.office-depot.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: office-depot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/office-depot/refs/heads/main/security/office-depot-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Office Supplies
- Retail
- B2B
- Fortune 500
---
