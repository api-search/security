---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: autotacbio.com
  spf: true
hosts:
- host: www.autotacbio.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autotacbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autotacbio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Autotacbio
provider_slug: autotacbio
slug: autotacbio-domain-security
source_filename: autotacbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autotacbio.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: autotacbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autotacbio/refs/heads/main/security/autotacbio-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Biotechnology
- Protein Degradation
- Therapeutics
- Korea
- AUTOTAC
---
