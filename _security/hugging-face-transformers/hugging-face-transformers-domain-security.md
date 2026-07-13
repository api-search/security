---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: huggingface.co
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: huggingface.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api-inference.huggingface.co
  https: false
kind: domain-security
layout: security
method: probed
name: Hugging Face Transformers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hugging Face Transformers, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hugging Face Transformers
provider_slug: hugging-face-transformers
slug: hugging-face-transformers-domain-security
source_filename: hugging-face-transformers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huggingface.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\n- host: api-inference.huggingface.co\n  https: false\ndomains:\n- domain: huggingface.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hugging-face-transformers/refs/heads/main/security/hugging-face-transformers-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Computer Vision
- Deep Learning
- Machine Learning
- Natural Language Processing
- Open Source
- Transformers
---
