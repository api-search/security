---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ruka.ai
  spf: true
hosts:
- cert_expires: Oct 18 00:14:58 2026 GMT
  host: ruka.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rukaai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ruka.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ruka.ai
provider_slug: rukaai
slug: rukaai-domain-security
source_filename: rukaai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ruka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 00:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ruka.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rukaai/refs/heads/main/security/rukaai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- Cost Optimization
- FinOps
- Operational Efficiency
- Invoice Processing
---
