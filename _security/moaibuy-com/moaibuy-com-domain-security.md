---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moaibuy.com
  spf: false
hosts:
- cert_expires: Jan 13 09:37:16 2027 GMT
  host: moaibuy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MoA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MoA
provider_slug: moaibuy-com
slug: moaibuy-com-domain-security
source_filename: moaibuy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moaibuy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 09:37:16 2027 GMT\n  hsts: false\ndomains:\n- domain: moaibuy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/moaibuy-com/security/moaibuy-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Marketplace
- Wholesale
- E-Commerce
- Korean
---
