---
api_specs:
- filename: overview
  format: yaml
  label: Parea REST API
  slug: parea-rest-api
  spec_type: OpenAPI
  url: https://docs.parea.ai/api-reference/overview
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parea.ai
  spf: true
- caa:
  - k8s-ingressn-ingressn-472382be57-0670a6c5b5c3bb3f.elb.us-east-2.amazonaws.com.
  dmarc: false
  dnssec: true
  domain: onporter.run
  spf: false
hosts:
- cert_expires: Sep 18 23:10:09 2026 GMT
  host: www.parea.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 14:24:03 2026 GMT
  host: docs.parea.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:50:06 2026 GMT
  host: parea-ai-backend-us-9ac16cdbc7a7b006.onporter.run
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parea AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parea AI
provider_slug: parea
slug: parea-domain-security
source_filename: parea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parea.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:10:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.parea.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:24:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: parea-ai-backend-us-9ac16cdbc7a7b006.onporter.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:50:06 2026 GMT\n  hsts: null\ndomains:\n- domain: parea.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: onporter.run\n  dnssec: true\n  caa:\n  - k8s-ingressn-ingressn-472382be57-0670a6c5b5c3bb3f.elb.us-east-2.amazonaws.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parea/refs/heads/main/security/parea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LLM
- Evaluation
- Observability
- Testing
- Prompt Management
- AI Engineering
- Machine Learning
- Tracing
- Experimentation
- Human Feedback
---
