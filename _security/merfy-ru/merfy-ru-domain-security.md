---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: merfy.ru
  spf: true
hosts:
- cert_expires: Jan 20 19:31:50 2027 GMT
  host: merfy.ru
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Merfy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merfy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Merfy
provider_slug: merfy-ru
slug: merfy-ru-domain-security
source_filename: merfy-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merfy.ru\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 19:31:50 2027 GMT\n  hsts: false\ndomains:\n- domain: merfy.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/merfy-ru/security/merfy-ru-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- E-Commerce
- Platform
- Online Store
- Consumer
- Russian
---
