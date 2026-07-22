---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: helpergo.co
  spf: true
hosts:
- cert_expires: Oct 11 07:42:25 2026 GMT
  host: helpergo.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helpergo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HelperGo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HelperGo
provider_slug: helpergo
slug: helpergo-domain-security
source_filename: helpergo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helpergo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:42:25 2026 GMT\n  hsts: false\ndomains:\n- domain: helpergo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helpergo/refs/heads/main/security/helpergo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Home Services
- Marketplace
- On-Demand
- Consumer
- Hong Kong
- Cleaning
- Childcare
---
