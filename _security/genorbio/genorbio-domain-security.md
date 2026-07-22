---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: genorbio.com
  spf: true
hosts:
- host: genorbio.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''genorbio.co'
kind: domain-security
layout: security
method: probed
name: Genorbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for genorbio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: genorbio
provider_slug: genorbio
slug: genorbio-domain-security
source_filename: genorbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genorbio.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''genorbio.co'\n  hsts: null\ndomains:\n- domain: genorbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genorbio/refs/heads/main/security/genorbio-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
