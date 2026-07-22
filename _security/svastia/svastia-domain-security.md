---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: svastia.ai
  spf: true
hosts:
- host: svastia.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Svastia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Svastia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Svastia
provider_slug: svastia
slug: svastia-domain-security
source_filename: svastia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: svastia.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: svastia.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/svastia/refs/heads/main/security/svastia-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Genomics
- Oncology
- Precision Medicine
- Bioinformatics
- Sequencing
- Clinical Trials
- Healthcare
- Life Sciences
- Cancer
---
