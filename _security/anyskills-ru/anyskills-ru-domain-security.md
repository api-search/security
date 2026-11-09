---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anyskills.ru
  spf: true
hosts:
- cert_expires: Jan 15 11:05:47 2027 GMT
  host: anyskills.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anyskills Ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnySkills, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AnySkills
provider_slug: anyskills-ru
slug: anyskills-ru-domain-security
source_filename: anyskills-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anyskills.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 11:05:47 2027 GMT\n  hsts: false\ndomains:\n- domain: anyskills.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anyskills-ru/security/anyskills-ru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- E-Learning
- Platform
- Course Management
- Russian
---
