---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: domob.cn
  spf: true
hosts:
- host: domob.cn
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''domob.cn''. '
kind: domain-security
layout: security
method: probed
name: Domob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for domob, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: domob
provider_slug: domob
slug: domob-domain-security
source_filename: domob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domob.cn\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''domob.cn''. '\n  hsts: null\ndomains:\n- domain: domob.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domob/refs/heads/main/security/domob-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Advertising
- Mobile
- AdTech
- Marketing
- SDK
- DSP
- Monetization
---
