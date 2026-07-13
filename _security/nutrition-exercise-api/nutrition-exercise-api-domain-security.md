---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dietagram.com
  spf: false
hosts:
- host: dietagram.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''dietagram.c'
kind: domain-security
layout: security
method: probed
name: Nutrition Exercise Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nutrition & Exercise API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Nutrition & Exercise API
provider_slug: nutrition-exercise-api
slug: nutrition-exercise-api-domain-security
source_filename: nutrition-exercise-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dietagram.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''dietagram.c'\n  hsts: null\ndomains:\n- domain: dietagram.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutrition-exercise-api/refs/heads/main/security/nutrition-exercise-api-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Exercise
- Food
- Health
- Nutrition
---
