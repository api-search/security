---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ohou.se
  spf: false
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: ohou.se
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ohouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OHouse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OHouse
provider_slug: ohouse
slug: ohouse-domain-security
source_filename: ohouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ohou.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ohou.se\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ohouse/refs/heads/main/security/ohouse-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ecommerce
---
