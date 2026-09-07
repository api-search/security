---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abderatx.com
  spf: true
hosts:
- host: www.abderatx.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abderatherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abdera Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abdera Therapeutics
provider_slug: abderatherapeutics
slug: abderatherapeutics-domain-security
source_filename: abderatherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abderatx.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: abderatx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abderatherapeutics/refs/heads/main/security/abderatherapeutics-domain-security.yml
summary_line: DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Radiopharmaceuticals
- Oncology
- Drug Development
- Clinical Trials
- Life Sciences
---
