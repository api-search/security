---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dizalpharma.com
  spf: true
hosts:
- cert_expires: Dec 21 05:41:47 2026 GMT
  host: www.dizalpharma.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dizal Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dizal Pharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dizal Pharma
provider_slug: dizal-pharma
slug: dizal-pharma-domain-security
source_filename: dizal-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dizalpharma.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 21 05:41:47 2026 GMT\n  hsts: false\ndomains:\n- domain: dizalpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dizal-pharma/refs/heads/main/security/dizal-pharma-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Healthcare
- Pharmaceutical
- Biotechnology
- Oncology
- Immunology
- Drug Development
- Clinical Research
- Life Sciences
---
