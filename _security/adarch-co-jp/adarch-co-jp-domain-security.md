---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adarch.co.jp
  spf: true
hosts:
- cert_expires: Apr 21 23:59:59 2027 GMT
  host: adarch.co.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adarch Co Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ad Arch株式会社, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ad Arch株式会社
provider_slug: adarch-co-jp
slug: adarch-co-jp-domain-security
source_filename: adarch-co-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adarch.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adarch.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/adarch-co-jp/security/adarch-co-jp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Media
- Video Production
- Marketing
- Japan
---
