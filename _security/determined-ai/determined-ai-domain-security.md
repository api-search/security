---
api_specs:
- filename: determined-ai-openapi.yml
  format: yaml
  label: Determined AI REST API
  slug: determined-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: determined.ai
  spf: true
hosts:
- host: www.determined.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.determi'
- host: docs.determined.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Determined Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Determined AI, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Determined AI
provider_slug: determined-ai
slug: determined-ai-domain-security
source_filename: determined-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.determined.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.determi'\n  hsts: null\n- host: docs.determined.ai\n  https: false\ndomains:\n- domain: determined.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/security/determined-ai-domain-security.yml
summary_line: DMARC
tags:
- Artificial Intelligence
- Deep Learning
- Machine Learning
- MLOps
---
