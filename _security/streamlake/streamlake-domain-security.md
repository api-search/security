---
api_specs:
- filename: streamlake-gateway-api-openapi.yml
  format: yaml
  label: StreamLake Gateway API
  slug: streamlake-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamlake/refs/heads/main/openapi/streamlake-gateway-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: streamlake.ai
  spf: false
hosts:
- cert_expires: Feb 22 03:32:45 2027 GMT
  host: streamlake.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 15 03:04:05 2026 GMT
  host: vanchin.streamlake.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Streamlake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StreamLake, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: StreamLake
provider_slug: streamlake
slug: streamlake-domain-security
source_filename: streamlake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: streamlake.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 03:32:45 2027 GMT\n  hsts: false\n- host: vanchin.streamlake.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 03:04:05 2026 GMT\n  hsts: false\ndomains:\n- domain: streamlake.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamlake/refs/heads/main/security/streamlake-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Artificial Intelligence
- LLM
- Model Inference
- Chat Completions
- AI Coding
- Kuaishou
---
