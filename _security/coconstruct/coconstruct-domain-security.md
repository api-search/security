---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coconstruct.com
  spf: true
hosts:
- cert_expires: Sep 10 20:02:29 2026 GMT
  host: www.coconstruct.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coconstruct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoConstruct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CoConstruct
provider_slug: coconstruct
slug: coconstruct-domain-security
source_filename: coconstruct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coconstruct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:02:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coconstruct.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coconstruct/refs/heads/main/security/coconstruct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Residential Construction
- Custom Home Builders
- Remodelers
- Construction Management
- Project Management
- Estimating
- Scheduling
- Client Collaboration
- Construction Financials
- SaaS
- Buildertrend
---
