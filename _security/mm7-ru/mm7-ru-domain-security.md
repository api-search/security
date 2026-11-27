---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mm7.ru
  spf: true
hosts:
- cert_expires: Feb 20 09:45:31 2027 GMT
  host: mm7.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ММ7 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ММ7, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ММ7
provider_slug: mm7-ru
slug: mm7-ru-domain-security
source_filename: mm7-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mm7.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 09:45:31 2027 GMT\n  hsts: false\ndomains:\n- domain: mm7.ru\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mm7-ru/security/mm7-ru-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- IT Services
- 1C Solutions
- Automation
- Russia
- Software Development
---
