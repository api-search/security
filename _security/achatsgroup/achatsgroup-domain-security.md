---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: achatsgroup.co.kr
  spf: true
hosts:
- host: achatsgroup.co.kr
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''achatsgroup'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Achatsgroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Achats Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Achats Group
provider_slug: achatsgroup
slug: achatsgroup-domain-security
source_filename: achatsgroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: achatsgroup.co.kr\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''achatsgroup'\n  hsts: null\ndomains:\n- domain: achatsgroup.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/achatsgroup/refs/heads/main/security/achatsgroup-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer Goods
- Media Commerce
- E-Commerce
- Direct to Consumer
- Cosmetics
- Health and Beauty
- Retail
- Cafe24
- South Korea
---
