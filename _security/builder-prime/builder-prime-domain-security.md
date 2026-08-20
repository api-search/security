---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: builderprime.com
  spf: true
hosts:
- cert_expires: Oct  1 14:02:08 2026 GMT
  host: www.builderprime.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: app.builderprime.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Builder Prime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Builder Prime, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Builder Prime
provider_slug: builder-prime
slug: builder-prime-domain-security
source_filename: builder-prime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.builderprime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:02:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.builderprime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: builderprime.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builder-prime/refs/heads/main/security/builder-prime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Home Improvement
- Construction
- Contractors
- Remodeling
- Sales
- Estimating
- Project Management
- Lead Management
- Field Service
- Software-as-a-Service
---
