---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hiddenlayer.com
  spf: true
hosts:
- cert_expires: Aug 30 06:37:34 2026 GMT
  host: hiddenlayer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hidden Layer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiddenLayer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HiddenLayer
provider_slug: hidden-layer
slug: hidden-layer-domain-security
source_filename: hidden-layer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hiddenlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:37:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hiddenlayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hidden-layer/refs/heads/main/security/hidden-layer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Security
- ML Security
- AISec
- AIDR
- AI Detection And Response
- AI Runtime Security
- Model Scanning
- AI Supply Chain
- AI Red Teaming
- Prompt Injection
- Jailbreak Detection
- AI Guardrails
- Agentic AI Security
- MCP Security
- Adversarial Machine Learning
- Generative AI Security
- Shadow AI
- AI Bill Of Materials
- Security
- Enterprise
---
