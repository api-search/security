---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rubriclabs.com
  spf: true
hosts:
- cert_expires: Aug 22 11:25:30 2026 GMT
  host: rubriclabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rubric Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rubric Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rubric Labs
provider_slug: rubric-ai
slug: rubric-ai-domain-security
source_filename: rubric-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rubriclabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:25:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rubriclabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubric-ai/refs/heads/main/security/rubric-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Applied AI
- Developer Tools
- Open Source
- Consulting
- LLM
---
