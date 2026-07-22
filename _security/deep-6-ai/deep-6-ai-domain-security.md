---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deep6.ai
  spf: true
hosts:
- host: deep6.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Deep 6 Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deep 6 AI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deep 6 AI
provider_slug: deep-6-ai
slug: deep-6-ai-domain-security
source_filename: deep-6-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deep6.ai\n  https: false\ndomains:\n- domain: deep6.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deep-6-ai/refs/heads/main/security/deep-6-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
- Clinical Trials
- Healthcare
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Electronic Health Records
- Precision Medicine
- Patient Matching
- Life Sciences
---
