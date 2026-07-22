---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mendel.ai
  spf: true
hosts:
- host: www.mendel.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Mendel Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mendel AI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mendel AI
provider_slug: mendel-ai
slug: mendel-ai-domain-security
source_filename: mendel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mendel.ai\n  https: false\ndomains:\n- domain: mendel.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mendel-ai/refs/heads/main/security/mendel-ai-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Clinical AI
- Healthcare AI
- Oncology
- Clinical Trials
- Patient Cohort Discovery
- Real World Data
- Electronic Health Records
- Natural Language Processing
- Large Language Models
- Clinical Knowledge Graph
- Pharmacovigilance
- Precision Medicine
- Life Sciences
---
