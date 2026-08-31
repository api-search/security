---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ausperbio.com
  spf: true
hosts:
- host: cn.ausperbio.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Cn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: cn
provider_slug: cn
slug: cn-domain-security
source_filename: cn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cn.ausperbio.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ausperbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cn/refs/heads/main/security/cn-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Biopharmaceutical
- Clinical-Stage
- Oligonucleotide Therapeutics
- Hepatitis B
- Drug Development
---
