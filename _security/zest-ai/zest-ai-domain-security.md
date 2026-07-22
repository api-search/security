---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zest.ai
  spf: true
hosts:
- cert_expires: Sep  8 12:08:38 2026 GMT
  host: zest.ai
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zest Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zest AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zest AI
provider_slug: zest-ai
slug: zest-ai-domain-security
source_filename: zest-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zest.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:08:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: zest.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zest-ai/refs/heads/main/security/zest-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lending
- Credit Underwriting
- Fraud Detection
- Artificial Intelligence
- Machine Learning
- Financial Services
- Fintech
---
