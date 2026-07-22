---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fox-tech.co
  spf: true
hosts:
- host: fox-tech.co
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Fox Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fox-Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fox-Tech
provider_slug: fox-tech
slug: fox-tech-domain-security
source_filename: fox-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fox-tech.co\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: fox-tech.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fox-tech/refs/heads/main/security/fox-tech-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- IoT
- Cold Chain
- Food Tech
- Supply Chain
- Agriculture
- Logistics
- Sensors
- Monitoring
- Taiwan
---
