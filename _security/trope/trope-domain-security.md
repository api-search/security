---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trope.ai
  spf: true
hosts:
- cert_expires: Oct 19 13:42:59 2026 GMT
  host: trope.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trope, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trope
provider_slug: trope
slug: trope-domain-security
source_filename: trope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trope.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 13:42:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trope.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trope/refs/heads/main/security/trope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- ERP
- Enterprise Software
- Computer Use
- MCP
- Automation
---
