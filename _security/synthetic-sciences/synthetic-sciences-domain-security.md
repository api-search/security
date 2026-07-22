---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: syntheticsciences.ai
  spf: true
hosts:
- cert_expires: Oct  4 05:42:50 2026 GMT
  host: syntheticsciences.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:37:28 2026 GMT
  host: docs.syntheticsciences.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 01:27:27 2026 GMT
  host: app.syntheticsciences.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synthetic Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthetic Sciences, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Synthetic Sciences
provider_slug: synthetic-sciences
slug: synthetic-sciences-domain-security
source_filename: synthetic-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syntheticsciences.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:42:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.syntheticsciences.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:37:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.syntheticsciences.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:27:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: syntheticsciences.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthetic-sciences/refs/heads/main/security/synthetic-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Scientific Research
- Developer Tools
- Agents
- Foundation Models
- Knowledge Graph
- Model Context Protocol
- CLI
- Research Infrastructure
---
