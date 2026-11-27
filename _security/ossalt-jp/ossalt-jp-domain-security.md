---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ossalt.jp
  spf: true
hosts:
- cert_expires: Jan  7 14:15:08 2027 GMT
  host: ossalt.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ossalt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ossalt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ossalt
provider_slug: ossalt-jp
slug: ossalt-jp-domain-security
source_filename: ossalt-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ossalt.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 14:15:08 2027 GMT\n  hsts: false\ndomains:\n- domain: ossalt.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ossalt-jp/security/ossalt-jp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Source Alternatives
- Japanese Teams
---
