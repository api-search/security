---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: byteroad.net
  spf: false
hosts:
- host: byteroad.net
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Byteroad Sociedade Unipessoal Lda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ByteRoad, Sociedade Unipessoal Lda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ByteRoad, Sociedade Unipessoal Lda
provider_slug: byteroad-sociedade-unipessoal-lda
slug: byteroad-sociedade-unipessoal-lda-domain-security
source_filename: byteroad-sociedade-unipessoal-lda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: byteroad.net\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: byteroad.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/byteroad-sociedade-unipessoal-lda/security/byteroad-sociedade-unipessoal-lda-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Road Safety
- IoT
- Data Analytics
- Transportation
---
