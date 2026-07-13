---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ust.hk
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.ust.hk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 02:04:04 2026 GMT
  host: hkust.developer.azure-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.ust.hk
  https: false
kind: domain-security
layout: security
method: probed
name: Hkust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hong Kong University of Science and Technology, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hong Kong University of Science and Technology
provider_slug: hkust
slug: hkust-domain-security
source_filename: hkust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ust.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: hkust.developer.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 02:04:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ust.hk\n  https: false\ndomains:\n- domain: ust.hk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hkust/refs/heads/main/security/hkust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Hong Kong
- China
---
