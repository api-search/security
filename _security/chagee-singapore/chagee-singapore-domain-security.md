---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chagee.com.sg
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.chagee.com.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chagee Singapore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CHAGEE Singapore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CHAGEE Singapore
provider_slug: chagee-singapore
slug: chagee-singapore-domain-security
source_filename: chagee-singapore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chagee.com.sg\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chagee.com.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/chagee-singapore/security/chagee-singapore-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Tea
- Beverage
- Singapore
- Retail
- Food
---
