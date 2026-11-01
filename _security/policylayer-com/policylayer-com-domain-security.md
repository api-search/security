---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: policylayer.com
  spf: false
hosts:
- cert_expires: Dec 23 21:22:59 2026 GMT
  host: policylayer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Policylayer Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for policylayer-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: policylayer-com
provider_slug: policylayer-com
slug: policylayer-com-domain-security
source_filename: policylayer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: policylayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 21:22:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: policylayer.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/policylayer-com/security/policylayer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Agent
- Policy
- Governance
- Automation
---
