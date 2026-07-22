---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frontier-communications.com
  spf: true
hosts:
- host: www.frontier-communications.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Frontier Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for frontier-communications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: frontier-communications
provider_slug: frontier-communications
slug: frontier-communications-domain-security
source_filename: frontier-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.frontier-communications.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: frontier-communications.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontier-communications/refs/heads/main/security/frontier-communications-domain-security.yml
summary_line: no transport/DNS hardening detected
tags: []
---
