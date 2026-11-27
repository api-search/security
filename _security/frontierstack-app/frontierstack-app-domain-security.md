---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: frontierstack.app
  spf: true
hosts:
- cert_expires: Jan 18 23:39:40 2027 GMT
  host: frontierstack.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Enfour, Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enfour, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Enfour, Inc.
provider_slug: frontierstack-app
slug: frontierstack-app-domain-security
source_filename: frontierstack-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frontierstack.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:39:40 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: frontierstack.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/frontierstack-app/security/frontierstack-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Server Management
- macOS
- AI Integration
- Fleet Administration
- Security
---
