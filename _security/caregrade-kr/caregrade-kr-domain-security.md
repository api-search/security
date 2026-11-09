---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caregrade.kr
  spf: false
hosts:
- cert_expires: Jan 10 14:01:22 2027 GMT
  host: caregrade.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caregrade Kr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 케어그레이드, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: 케어그레이드
provider_slug: caregrade-kr
slug: caregrade-kr-domain-security
source_filename: caregrade-kr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caregrade.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 14:01:22 2027 GMT\n  hsts: false\ndomains:\n- domain: caregrade.kr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/caregrade-kr/security/caregrade-kr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Data
- South Korea
- Long-Term Care
- Public
---
