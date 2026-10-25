---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: australiansuper.com
  spf: true
hosts:
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: australiansuper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Australiansuper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AustralianSuper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AustralianSuper
provider_slug: australiansuper
slug: australiansuper-domain-security
source_filename: australiansuper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: australiansuper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: australiansuper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australiansuper/refs/heads/main/security/australiansuper-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Superannuation
- Retirement
- Financial Services
- Investment Management
- Pension Funds
- Australia
---
