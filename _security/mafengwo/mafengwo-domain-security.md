---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mafengwo.cn
  spf: true
hosts:
- host: mafengwo.cn
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''mafengwo.cn'
kind: domain-security
layout: security
method: probed
name: Mafengwo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mafengwo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mafengwo
provider_slug: mafengwo
slug: mafengwo-domain-security
source_filename: mafengwo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mafengwo.cn\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''mafengwo.cn'\n  hsts: null\ndomains:\n- domain: mafengwo.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mafengwo/refs/heads/main/security/mafengwo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Travel
- Tourism
- China
- Community
- User-Generated Content
- Reviews
- Travel Guides
- Booking
---
