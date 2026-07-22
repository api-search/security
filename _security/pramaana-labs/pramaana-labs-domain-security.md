---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pramaanalabs.ai
  spf: true
hosts:
- cert_expires: Sep 28 04:10:53 2026 GMT
  host: pramaanalabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pramaana Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pramaana Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pramaana Labs
provider_slug: pramaana-labs
slug: pramaana-labs-domain-security
source_filename: pramaana-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pramaanalabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:10:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pramaanalabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pramaana-labs/refs/heads/main/security/pramaana-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Verification
- Formal Methods
- Machine Learning
- Research
- Compiler
- LLM
- Reasoning
---
