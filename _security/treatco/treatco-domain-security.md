---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: treat.co
  spf: true
hosts:
- host: treat.co
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''treat.co''. '
kind: domain-security
layout: security
method: probed
name: Treatco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treat.co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Treat.co
provider_slug: treatco
slug: treatco-domain-security
source_filename: treatco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: treat.co\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''treat.co''. '\n  hsts: null\ndomains:\n- domain: treat.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treatco/refs/heads/main/security/treatco-domain-security.yml
summary_line: DMARC
tags:
- Company
- Gifting
- E-Commerce
- Consumer
- Retail
- Confectionery
---
