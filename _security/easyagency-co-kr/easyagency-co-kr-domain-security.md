---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easyagency.co.kr
  spf: false
hosts:
- cert_expires: Jan  4 04:55:33 2027 GMT
  host: easyagency.co.kr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 이지에이전시 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 이지에이전시, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: 이지에이전시
provider_slug: easyagency-co-kr
slug: easyagency-co-kr-domain-security
source_filename: easyagency-co-kr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easyagency.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 04:55:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: easyagency.co.kr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/easyagency-co-kr/security/easyagency-co-kr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Development
- Marketing
- Branding
- Content Creation
- South Korea
---
