---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brexogen.com
  spf: true
hosts:
- host: brexogen.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brexogen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brexogen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Brexogen
provider_slug: brexogen
slug: brexogen-domain-security
source_filename: brexogen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brexogen.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: brexogen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brexogen/refs/heads/main/security/brexogen-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Therapeutics
- Exosomes
- Healthcare
---
