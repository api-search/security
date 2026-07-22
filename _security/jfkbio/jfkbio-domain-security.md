---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jfkbio.com
  spf: true
hosts:
- host: jfkbio.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Jfkbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jfkbio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: jfkbio
provider_slug: jfkbio
slug: jfkbio-domain-security
source_filename: jfkbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jfkbio.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: jfkbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jfkbio/refs/heads/main/security/jfkbio-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Life Sciences
- Healthcare
- Pharmaceuticals
- China
---
