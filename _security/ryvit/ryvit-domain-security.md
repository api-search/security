---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ryvit.com
  spf: false
hosts:
- host: ryvit.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''ryvit.com''.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ryvit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ryvit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ryvit
provider_slug: ryvit
slug: ryvit-domain-security
source_filename: ryvit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ryvit.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''ryvit.com''.'\n  hsts: null\ndomains:\n- domain: ryvit.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ryvit/security/ryvit-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Renewable Energy
- Asset Management
- Data Analytics
- Predictive Maintenance
---
