---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bonsave.app
  spf: true
hosts:
- cert_expires: Dec 25 23:11:29 2026 GMT
  host: bonsave.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bonsave App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonsave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bonsave
provider_slug: bonsave-app
slug: bonsave-app-domain-security
source_filename: bonsave-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bonsave.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bonsave.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bonsave-app/security/bonsave-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Planning
- Net Worth Tracking
- AI Insights
- Retirement Planning
- Investment Tracking
---
