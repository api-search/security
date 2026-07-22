---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: belvedir.ai
  spf: false
hosts:
- cert_expires: Oct 10 07:54:21 2026 GMT
  host: belvedir.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Belvedir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belvedir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Belvedir
provider_slug: belvedir
slug: belvedir-domain-security
source_filename: belvedir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: belvedir.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 07:54:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: belvedir.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belvedir/refs/heads/main/security/belvedir-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Reinforcement Learning
- Private AI
- Fine-Tuning
- LLM
- Agents
- Model Hosting
---
