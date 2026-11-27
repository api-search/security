---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zaif.jp
  spf: true
hosts:
- cert_expires: Apr  3 05:31:21 2027 GMT
  host: zaif.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zaif Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zaif, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zaif
provider_slug: zaif
slug: zaif-domain-security
source_filename: zaif-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zaif.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  3 05:31:21 2027 GMT\n  hsts: false\ndomains:\n- domain: zaif.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/zaif/security/zaif-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Automatic Trading
- Staking
- Payment Card
---
