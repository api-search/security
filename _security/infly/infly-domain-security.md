---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: infly.cn
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: infly.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Infly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INF Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: INF Tech
provider_slug: infly
slug: infly-domain-security
source_filename: infly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infly.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infly.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infly/refs/heads/main/security/infly-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Generative AI
- AI Agents
- Document Parsing
- Retrieval
- Finance
---
