---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ibtcc.kr
  spf: false
hosts:
- cert_expires: Jan 15 08:11:31 2027 GMT
  host: ibtcc.kr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IBTCC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBTCC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: IBTCC
provider_slug: ibtcc-kr
slug: ibtcc-kr-domain-security
source_filename: ibtcc-kr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ibtcc.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 08:11:31 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ibtcc.kr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ibtcc-kr/security/ibtcc-kr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Recruiting
- Public Sector
- South Korea
- Job Search
---
