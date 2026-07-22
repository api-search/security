---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: goodpeople.com
  spf: false
hosts:
- cert_expires: Aug 22 07:31:17 2026 GMT
  host: goodpeople.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Arg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ARG
provider_slug: arg
slug: arg-domain-security
source_filename: arg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goodpeople.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 07:31:17 2026 GMT\n  hsts: false\ndomains:\n- domain: goodpeople.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arg/refs/heads/main/security/arg-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Community
- Sports
- Snowboarding
- Skiing
- Freeride
- Events
- Ecommerce
- Lifestyle
---
