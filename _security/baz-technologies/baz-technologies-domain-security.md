---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: baz.ai
  spf: true
hosts:
- cert_expires: Sep 29 15:52:48 2026 GMT
  host: baz.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baz Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baz Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Baz Technologies
provider_slug: baz-technologies
slug: baz-technologies-domain-security
source_filename: baz-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baz.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:52:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: baz.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baz-technologies/refs/heads/main/security/baz-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Code Review
- Developer Tools
- AI Agents
- Application Security
- Agentic Coding
- DevOps
- Model Context Protocol
- Software Engineering
---
