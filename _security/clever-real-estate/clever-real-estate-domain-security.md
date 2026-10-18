---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cleverrealtors.com
  spf: true
hosts:
- cert_expires: Dec 10 13:40:41 2026 GMT
  host: cleverrealtors.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clever Real Estate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clever Real Estate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clever Real Estate
provider_slug: clever-real-estate
slug: clever-real-estate-domain-security
source_filename: clever-real-estate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cleverrealtors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 13:40:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cleverrealtors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clever-real-estate/refs/heads/main/security/clever-real-estate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Brokerage
- Dallas
- Low Commission
---
