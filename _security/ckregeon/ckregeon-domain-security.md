---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ckregeon.com
  spf: true
hosts:
- host: ckregeon.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ckregeon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ckregeon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ckregeon
provider_slug: ckregeon
slug: ckregeon-domain-security
source_filename: ckregeon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ckregeon.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ckregeon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ckregeon/refs/heads/main/security/ckregeon-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Biotechnology
- Drug Development
- Platform Technology
- Screening Systems
- Chemical Synthesis
- Disease Targets
---
