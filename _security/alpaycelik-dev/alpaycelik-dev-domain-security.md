---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alpaycelik.dev
  spf: true
hosts:
- cert_expires: Dec 16 18:59:10 2026 GMT
  host: alpaycelik.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alpaycelik Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpay Celik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alpay Celik
provider_slug: alpaycelik-dev
slug: alpaycelik-dev-domain-security
source_filename: alpaycelik-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alpaycelik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 18:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alpaycelik.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/alpaycelik-dev/security/alpaycelik-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Full-Stack
- Engineer
- Germany
- Software Development
- Portfolio
---
