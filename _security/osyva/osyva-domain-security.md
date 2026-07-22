---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: osyva.com
  spf: true
hosts:
- host: osyva.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''osyva.com''.'
kind: domain-security
layout: security
method: probed
name: Osyva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osyva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Osyva
provider_slug: osyva
slug: osyva-domain-security
source_filename: osyva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osyva.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''osyva.com''.'\n  hsts: null\ndomains:\n- domain: osyva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osyva/refs/heads/main/security/osyva-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Veterinary
- B2B Commerce
- Procurement
- E-Commerce
- Distribution
- Agtech
- Latin America
- Colombia
---
