---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: reevl.co.kr
  spf: true
hosts:
- cert_expires: Feb 14 22:32:44 2027 GMT
  host: reevl.co.kr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 리블 (Reevl) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 리블 (Reevl), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 리블 (Reevl)
provider_slug: reevl-co-kr
slug: reevl-co-kr-domain-security
source_filename: reevl-co-kr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reevl.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 22:32:44 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: reevl.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reevl-co-kr/security/reevl-co-kr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Analytics
- AI
- South Korea
- Property Data
---
