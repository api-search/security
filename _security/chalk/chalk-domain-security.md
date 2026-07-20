---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chalk.ai
  spf: true
hosts:
- cert_expires: Sep 24 10:58:42 2026 GMT
  host: chalk.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chalk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chalk
provider_slug: chalk
slug: chalk-domain-security
source_filename: chalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chalk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:58:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chalk.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chalk/refs/heads/main/security/chalk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Machine Learning
- Feature Store
- Artificial Intelligence
- Data Platform
- MLOps
- Real-Time Data
- LLM
- Agents
- Feature Engineering
---
