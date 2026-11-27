---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: index-now.ru
  spf: true
hosts:
- cert_expires: Feb  1 20:11:54 2027 GMT
  host: index-now.ru
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: index-now-ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for index-now-ru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: index-now-ru
provider_slug: index-now-ru
slug: index-now-ru-domain-security
source_filename: index-now-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: index-now.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 20:11:54 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: index-now.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/index-now-ru/security/index-now-ru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- Indexing
- Webmaster Tools
---
