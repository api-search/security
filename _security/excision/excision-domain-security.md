---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: excision.bio
  spf: true
hosts:
- host: excision.bio
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Excision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Excision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Excision
provider_slug: excision
slug: excision-domain-security
source_filename: excision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: excision.bio\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: excision.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/excision/refs/heads/main/security/excision-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- CRISPR
- Gene Editing
- Therapeutics
- Life Sciences
- Infectious Disease
- Venture Backed
---
