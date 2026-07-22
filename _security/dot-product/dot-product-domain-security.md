---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: dotproduct.xyz
  spf: false
hosts:
- host: dotproduct.xyz
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''dotproduct.'
kind: domain-security
layout: security
method: probed
name: Dot Product Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dot Product, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Dot Product
provider_slug: dot-product
slug: dot-product-domain-security
source_filename: dot-product-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dotproduct.xyz\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''dotproduct.'\n  hsts: null\ndomains:\n- domain: dotproduct.xyz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dot-product/refs/heads/main/security/dot-product-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Voice Agents
- Customer Support
- Operations
- AI Agents
- Conversational AI
---
