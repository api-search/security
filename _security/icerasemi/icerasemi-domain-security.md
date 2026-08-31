---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: icerasemi.com
  spf: true
hosts:
- host: www.icerasemi.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.icerase'
kind: domain-security
layout: security
method: probed
name: Icerasemi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for icerasemi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: icerasemi
provider_slug: icerasemi
slug: icerasemi-domain-security
source_filename: icerasemi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icerasemi.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.icerase'\n  hsts: null\ndomains:\n- domain: icerasemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icerasemi/refs/heads/main/security/icerasemi-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Semiconductor
- Modem
- Wireless
- Fabless
---
