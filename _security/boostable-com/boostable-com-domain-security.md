---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boostable.com
  spf: true
hosts:
- host: boostable.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''boostable.c'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boostable Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adjoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Adjoint
provider_slug: boostable-com
slug: boostable-com-domain-security
source_filename: boostable-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boostable.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''boostable.c'\n  hsts: null\ndomains:\n- domain: boostable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/boostable-com/security/boostable-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- AI
- Optimization
- Analytics
- Enterprise
---
