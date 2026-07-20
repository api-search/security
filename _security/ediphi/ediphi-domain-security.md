---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ediphi.com
  spf: true
hosts:
- cert_expires: Oct  7 08:17:07 2026 GMT
  host: ediphi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 19:58:06 2026 GMT
  host: help.ediphi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: api.ediphi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ediphi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ediphi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ediphi
provider_slug: ediphi
slug: ediphi-domain-security
source_filename: ediphi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ediphi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:17:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.ediphi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:58:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ediphi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ediphi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ediphi/refs/heads/main/security/ediphi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Preconstruction
- Cost Estimating
- Construction Technology
- Estimating
- Cost Management
- SaaS
---
