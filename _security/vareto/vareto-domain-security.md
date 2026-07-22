---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vareto.com
  spf: true
hosts:
- cert_expires: Aug 29 09:47:44 2026 GMT
  host: vareto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vareto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vareto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vareto
provider_slug: vareto
slug: vareto-domain-security
source_filename: vareto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vareto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 09:47:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vareto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vareto/refs/heads/main/security/vareto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Finance
- FP&A
- Financial Planning
- Forecasting
- Budgeting
- SaaS
---
