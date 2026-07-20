---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infini-ai.com
  spf: true
hosts:
- cert_expires: Oct 16 23:01:49 2026 GMT
  host: docs.infini-ai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infini-AI (无问芯穹), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Infini-AI (无问芯穹)
provider_slug: docs
slug: docs-domain-security
source_filename: docs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.infini-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:01:49 2026 GMT\n  hsts: false\ndomains:\n- domain: infini-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docs/refs/heads/main/security/docs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Model as a Service
- Inference
- ComfyUI
- Agents
- AGI Compute
- OpenAI-Compatible
---
