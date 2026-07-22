---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: baycon.co.kr
  spf: true
hosts:
- host: baycon.co.kr
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Baycon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BAYCON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BAYCON
provider_slug: baycon
slug: baycon-domain-security
source_filename: baycon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baycon.co.kr\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: baycon.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baycon/refs/heads/main/security/baycon-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- eSIM
- Telecommunications
- Connectivity
- Travel
- VoIP
- Mobile
- Roaming
- Korea
---
