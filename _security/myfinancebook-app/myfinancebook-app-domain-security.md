---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myfinancebook.app
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: myfinancebook.app
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MyFinanceBook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyFinanceBook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyFinanceBook
provider_slug: myfinancebook-app
slug: myfinancebook-app-domain-security
source_filename: myfinancebook-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myfinancebook.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: myfinancebook.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/myfinancebook-app/security/myfinancebook-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Artificial Intelligence
- Personal Finance
- Budgeting
- Privacy
---
