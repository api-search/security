---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kitemir.jp
  spf: true
hosts:
- cert_expires: Mar  4 06:30:51 2027 GMT
  host: kitemir.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: StyleAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StyleAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: StyleAI
provider_slug: kitemir-jp
slug: kitemir-jp-domain-security
source_filename: kitemir-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kitemir.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 06:30:51 2027 GMT\n  hsts: false\ndomains:\n- domain: kitemir.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kitemir-jp/security/kitemir-jp-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Fashion
- Virtual Try-On
- PersonalColor
---
