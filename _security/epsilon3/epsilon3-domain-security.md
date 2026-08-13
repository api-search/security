---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: epsilon3.io
  spf: true
hosts:
- cert_expires: Oct  3 23:31:17 2026 GMT
  host: www.epsilon3.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: docs.epsilon3.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: api.epsilon3.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Epsilon3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epsilon3, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Epsilon3
provider_slug: epsilon3
slug: epsilon3-domain-security
source_filename: epsilon3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epsilon3.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:31:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.epsilon3.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n- host: api.epsilon3.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epsilon3.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epsilon3/refs/heads/main/security/epsilon3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Operations
- Aerospace
- Space
- Defense
- Manufacturing
- Procedures
- Workflow
- Inventory
- Telemetry
- Test Management
- Project Management
- MCP
---
