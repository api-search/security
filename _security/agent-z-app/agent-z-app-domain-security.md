---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agent-z.app
  spf: true
hosts:
- cert_expires: Dec 30 20:16:01 2026 GMT
  host: agent-z.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EDGE Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EDGE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EDGE
provider_slug: agent-z-app
slug: agent-z-app-domain-security
source_filename: agent-z-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-z.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 20:16:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agent-z.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agent-z-app/security/agent-z-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Cryptocurrency
- Trading
- Automation
- Tokenization
---
