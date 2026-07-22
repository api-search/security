---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: doc.ai
  spf: true
hosts:
- host: doc.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Docai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for doc.ai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: doc.ai
provider_slug: docai
slug: docai-domain-security
source_filename: docai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doc.ai\n  https: false\ndomains:\n- domain: doc.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docai/refs/heads/main/security/docai-domain-security.yml
summary_line: DMARC
tags:
- Company
- Crypto
- Artificial Intelligence
- Health
- Digital Health
- Machine Learning
- Tokens
- Defunct
- Acquired
---
