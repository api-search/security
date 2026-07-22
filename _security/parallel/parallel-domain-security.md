---
api_specs:
- filename: parallel-openapi-original.json
  format: json
  label: Parallel API
  slug: parallel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parallel.ai
  spf: true
hosts:
- cert_expires: Aug 25 17:19:34 2026 GMT
  host: www.parallel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 19:46:36 2026 GMT
  host: api.parallel.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parallel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parallel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parallel
provider_slug: parallel
slug: parallel-domain-security
source_filename: parallel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parallel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.parallel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:46:36 2026 GMT\n  hsts: null\ndomains:\n- domain: parallel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/security/parallel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Web Search
- Agents
- Deep Research
- Web Extraction
- Data Enrichment
- Web Monitoring
- LLM Tools
---
