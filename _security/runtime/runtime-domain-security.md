---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: runtm.com
  spf: false
hosts:
- cert_expires: Sep 22 10:39:53 2026 GMT
  host: www.runtm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 10:39:53 2026 GMT
  host: docs.runtm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 11:30:17 2026 GMT
  host: app.runtm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runtime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Runtime, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Runtime
provider_slug: runtime
slug: runtime-domain-security
source_filename: runtime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.runtm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:39:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.runtm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:39:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.runtm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:30:17 2026 GMT\n  hsts: false\ndomains:\n- domain: runtm.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runtime/refs/heads/main/security/runtime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Coding Agents
- Developer Tools
- AI Infrastructure
- Sandboxes
- Agent Orchestration
- DevOps
- Cloud
---
