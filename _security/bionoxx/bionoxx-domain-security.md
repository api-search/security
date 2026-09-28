---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bionoxx.com
  spf: true
hosts:
- host: bionoxx.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bionoxx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bionoxx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bionoxx
provider_slug: bionoxx
slug: bionoxx-domain-security
source_filename: bionoxx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bionoxx.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: bionoxx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bionoxx/refs/heads/main/security/bionoxx-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- MolecularDiagnostics
- Bioinformatics
- HealthTech
---
