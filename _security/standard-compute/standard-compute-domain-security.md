---
api_specs:
- filename: standard-compute-openapi.json
  format: json
  label: Standard Compute Inference API
  slug: standard-compute-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: standardcompute.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: stdcmpt.com
  spf: false
hosts:
- cert_expires: Oct 24 17:51:14 2026 GMT
  host: standardcompute.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 16:42:53 2026 GMT
  host: api.stdcmpt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Standard Compute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standard Compute, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Standard Compute
provider_slug: standard-compute
slug: standard-compute-domain-security
source_filename: standard-compute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standardcompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 17:51:14 2026 GMT\n  hsts: false\n- host: api.stdcmpt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 16:42:53 2026 GMT\n  hsts: null\ndomains:\n- domain: standardcompute.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stdcmpt.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/security/standard-compute-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- llm api
- flat-rate
- subscription
- ai agents
- inference
- model routing
- ai gateway
- developer tools
- coding agents
- openai-compatible
---
