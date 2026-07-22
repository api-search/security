---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: opensesame.com
  spf: true
hosts:
- cert_expires: Jan  9 23:06:34 2027 GMT
  host: opensesame.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opensesame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opensesame, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Opensesame
provider_slug: opensesame
slug: opensesame-domain-security
source_filename: opensesame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opensesame.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:06:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opensesame.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensesame/refs/heads/main/security/opensesame-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- eLearning
- Learning Management
- Online Training
- Course Marketplace
- Corporate Training
- LMS Integration
- xAPI
- Applicative Saas
---
