---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tenex.io
  spf: false
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: tenex.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tenex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tenex
provider_slug: tenex
slug: tenex-domain-security
source_filename: tenex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tenex.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tenex.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenex/refs/heads/main/security/tenex-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- PropTech
- Real Estate
- Property Management
- Facility Management
- Tenant Experience
- Hospitality
- Accounting
- GCC
- SaaS
---
