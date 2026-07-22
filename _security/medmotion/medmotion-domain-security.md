---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medmotion.cn
  spf: true
hosts:
- host: medmotion.cn
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''medmotion.c'
kind: domain-security
layout: security
method: probed
name: Medmotion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for medmotion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: medmotion
provider_slug: medmotion
slug: medmotion-domain-security
source_filename: medmotion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medmotion.cn\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''medmotion.c'\n  hsts: null\ndomains:\n- domain: medmotion.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medmotion/refs/heads/main/security/medmotion-domain-security.yml
summary_line: DMARC
tags:
- Company
- Healthcare
- Medical
- Rehabilitation
- Orthopedics
- Digital Therapeutics
- Sports Medicine
- China
---
