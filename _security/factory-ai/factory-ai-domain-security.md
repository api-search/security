---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: factory.ai
  spf: true
hosts:
- cert_expires: Aug 25 17:44:19 2026 GMT
  host: factory.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 23:27:47 2026 GMT
  host: app.factory.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Factory Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Factory, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Factory
provider_slug: factory-ai
slug: factory-ai-domain-security
source_filename: factory-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: factory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:44:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.factory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:27:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: factory.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factory-ai/refs/heads/main/security/factory-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Agents
- Autonomous
- Developer Tools
- Software Engineering
- Code Generation
- DevOps
---
