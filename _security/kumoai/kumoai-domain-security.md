---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kumo.ai
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: kumo.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kumoai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kumo.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kumo.AI
provider_slug: kumoai
slug: kumoai-domain-security
source_filename: kumoai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kumo.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: kumo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kumoai/refs/heads/main/security/kumoai-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Ai
- Machine Learning
- Predictive Analytics
- Graph Neural Networks
- Foundation Models
- Data Warehouse
- Model Context Protocol
- Agents
- Relational Data
---
