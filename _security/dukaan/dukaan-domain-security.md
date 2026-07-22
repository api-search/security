---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mydukaan.io
  spf: true
hosts:
- cert_expires: Aug  5 13:10:54 2026 GMT
  host: mydukaan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dukaan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dukaan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dukaan
provider_slug: dukaan
slug: dukaan-domain-security
source_filename: dukaan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mydukaan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 13:10:54 2026 GMT\n  hsts: false\ndomains:\n- domain: mydukaan.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dukaan/refs/heads/main/security/dukaan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Online Store
- Store Builder
- Retail
- Themes
- Templating
- Plugins
- Logistics
- India
---
