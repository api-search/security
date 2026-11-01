---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: catalyst.io
  spf: false
hosts:
- cert_expires: Dec  9 17:01:48 2026 GMT
  host: www.catalyst.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getcatalyst Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catalyst, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Catalyst
provider_slug: getcatalyst-io
slug: getcatalyst-io-domain-security
source_filename: getcatalyst-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.catalyst.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 17:01:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: catalyst.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getcatalyst-io/security/getcatalyst-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- SaaS
- Customer Success
- Platform
- Automation
---
