---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: seriousenergy.com
  spf: true
hosts:
- host: www.seriousenergy.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Serious Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serious Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Serious Energy
provider_slug: serious-energy
slug: serious-energy-domain-security
source_filename: serious-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seriousenergy.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: seriousenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/serious-energy/security/serious-energy-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
