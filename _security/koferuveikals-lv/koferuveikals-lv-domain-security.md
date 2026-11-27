---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: koferuveikals.lv
  spf: true
hosts:
- cert_expires: Jan  9 19:06:40 2027 GMT
  host: koferuveikals.lv
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Koferuveikals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koferuveikals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Koferuveikals
provider_slug: koferuveikals-lv
slug: koferuveikals-lv-domain-security
source_filename: koferuveikals-lv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koferuveikals.lv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 19:06:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: koferuveikals.lv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/koferuveikals-lv/security/koferuveikals-lv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
