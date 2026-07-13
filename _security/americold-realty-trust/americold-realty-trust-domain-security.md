---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: americold.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: i-3pl.com
  spf: false
hosts:
- cert_expires: Aug 18 07:44:23 2026 GMT
  host: www.americold.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: www.i-3pl.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Americold Realty Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Americold Realty Trust, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Americold Realty Trust
provider_slug: americold-realty-trust
slug: americold-realty-trust-domain-security
source_filename: americold-realty-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.americold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 07:44:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.i-3pl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: americold.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: i-3pl.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/americold-realty-trust/refs/heads/main/security/americold-realty-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cold Storage
- Logistics
- Supply Chain
- Warehousing
- Real Estate
- Temperature-Controlled
- Cold Chain
- EDI
- 3PL
---
