---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: stailer.jp
  spf: false
hosts:
- cert_expires: Dec 16 02:57:02 2026 GMT
  host: stailer.jp
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stailer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stailer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Stailer
provider_slug: stailer
slug: stailer-domain-security
source_filename: stailer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stailer.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 02:57:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: stailer.jp\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stailer/refs/heads/main/security/stailer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Retail
- E-commerce
- Grocery
- Japan
- SaaS
- Digital Transformation
---
