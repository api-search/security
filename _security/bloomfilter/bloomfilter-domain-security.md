---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bloomfilter.ai
  spf: true
hosts:
- cert_expires: Oct 13 09:25:57 2026 GMT
  host: www.bloomfilter.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomfilter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomfilter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bloomfilter
provider_slug: bloomfilter
slug: bloomfilter-domain-security
source_filename: bloomfilter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomfilter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 09:25:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bloomfilter.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomfilter/refs/heads/main/security/bloomfilter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Process Intelligence
- Software Development Lifecycle
- AI Agents
- Agent Governance
- Process Mining
- Observability
- Compliance
- Workflow Automation
- DevOps
---
