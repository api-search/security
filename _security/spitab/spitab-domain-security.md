---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spitab.com
  spf: false
hosts:
- host: www.spitab.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.spitab.'
kind: domain-security
layout: security
method: probed
name: Spitab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spitab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Spitab
provider_slug: spitab
slug: spitab-domain-security
source_filename: spitab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spitab.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.spitab.'\n  hsts: null\ndomains:\n- domain: spitab.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spitab/refs/heads/main/security/spitab-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- API
- Digital Services
---
