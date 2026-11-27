---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ntable.kr
  spf: true
hosts:
- cert_expires: Jan  5 05:09:42 2027 GMT
  host: ntable.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ntable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ntable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ntable
provider_slug: ntable-kr
slug: ntable-kr-domain-security
source_filename: ntable-kr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ntable.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:09:42 2027 GMT\n  hsts: false\ndomains:\n- domain: ntable.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ntable-kr/security/ntable-kr-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Meeting
- Facilitation
- Collaboration
- Productivity
---
