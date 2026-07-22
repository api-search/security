---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: efishery.com
  spf: true
hosts:
- host: efishery.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''efishery.co'
kind: domain-security
layout: security
method: probed
name: Efishery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eFishery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: eFishery
provider_slug: efishery
slug: efishery-domain-security
source_filename: efishery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: efishery.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''efishery.co'\n  hsts: null\ndomains:\n- domain: efishery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/efishery/refs/heads/main/security/efishery-domain-security.yml
summary_line: DMARC
tags:
- Company
- Aquaculture
- AgriTech
- FishTech
- IoT
- FinTech
- Marketplace
- Smart Feeder
- Indonesia
---
