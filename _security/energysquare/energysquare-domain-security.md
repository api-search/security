---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: energysquare.co
  spf: true
hosts:
- host: energysquare.co
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''energysquar'
kind: domain-security
layout: security
method: probed
name: Energysquare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Energysquare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Energysquare
provider_slug: energysquare
slug: energysquare-domain-security
source_filename: energysquare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: energysquare.co\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''energysquar'\n  hsts: null\ndomains:\n- domain: energysquare.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energysquare/refs/heads/main/security/energysquare-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Industrial, Energy & Iot
---
