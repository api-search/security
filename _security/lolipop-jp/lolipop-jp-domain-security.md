---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lolipop.jp
  spf: true
hosts:
- cert_expires: Apr 30 02:43:31 2027 GMT
  host: lolipop.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ロリポップ！レンタルサーバー Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ロリポップ！レンタルサーバー, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ロリポップ！レンタルサーバー
provider_slug: lolipop-jp
slug: lolipop-jp-domain-security
source_filename: lolipop-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lolipop.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 30 02:43:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lolipop.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lolipop-jp/security/lolipop-jp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hosting
- Cloud
- Japanese
- Web
- Software-as-a-Service
- Company
---
