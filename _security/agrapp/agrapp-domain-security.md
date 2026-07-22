---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agrapp.cl
  spf: true
hosts:
- cert_expires: Oct 14 10:25:59 2026 GMT
  host: agrapp.cl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agrapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agrapp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agrapp
provider_slug: agrapp
slug: agrapp-domain-security
source_filename: agrapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agrapp.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 10:25:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agrapp.cl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrapp/refs/heads/main/security/agrapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- AgTech
- Farm Management
- SaaS
- Chile
- Latin America
- Mobile
---
