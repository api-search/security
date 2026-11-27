---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: podpisator.ru
  spf: true
hosts:
- cert_expires: Jan 10 06:24:58 2027 GMT
  host: podpisator.ru
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Подписатор Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Подписатор, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Подписатор
provider_slug: iipodpis-ru
slug: iipodpis-ru-domain-security
source_filename: iipodpis-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podpisator.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 06:24:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: podpisator.ru\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/iipodpis-ru/security/iipodpis-ru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Signature
- Online Tool
- Free
- Russian
---
