---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dashamail.ru
  spf: true
hosts:
- cert_expires: Jan 31 10:32:35 2027 GMT
  host: dashamail.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dashamail Ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DashaMail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DashaMail
provider_slug: dashamail-ru
slug: dashamail-ru-domain-security
source_filename: dashamail-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dashamail.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 10:32:35 2027 GMT\n  hsts: false\ndomains:\n- domain: dashamail.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dashamail-ru/security/dashamail-ru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- Marketing
- Automation
- Russian
---
