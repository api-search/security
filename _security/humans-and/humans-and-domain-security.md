---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: humansand.ai
  spf: true
hosts:
- cert_expires: Oct 14 14:04:18 2026 GMT
  host: humansand.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humans And Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humans&, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Humans&
provider_slug: humans-and
slug: humans-and-domain-security
source_filename: humans-and-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humansand.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 14:04:18 2026 GMT\n  hsts: false\ndomains:\n- domain: humansand.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humans-and/refs/heads/main/security/humans-and-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Frontier AI
- Research Lab
- Multi-Agent Systems
- Reinforcement Learning
---
