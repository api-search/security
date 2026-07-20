---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imandra.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imandrax.dev
  spf: false
hosts:
- cert_expires: Sep  5 19:23:00 2026 GMT
  host: www.imandra.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 01:32:20 2026 GMT
  host: imandrax.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 19:23:00 2026 GMT
  host: universe.imandra.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imandra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imandra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Imandra
provider_slug: imandra
slug: imandra-domain-security
source_filename: imandra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.imandra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:23:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: imandrax.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:32:20 2026 GMT\n  hsts: false\n- host: universe.imandra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:23:00 2026 GMT\n  hsts: null\ndomains:\n- domain: imandra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: imandrax.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imandra/refs/heads/main/security/imandra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Automated Reasoning
- Formal Verification
- Theorem Proving
- Developer Tools
- Code Analysis
- Financial Services
- gRPC
- MCP
---
