---
api_specs:
- filename: priorlabs-openapi-original.json
  format: json
  label: TabPFN API
  slug: tabpfn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/priorlabs/refs/heads/main/openapi/priorlabs-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: priorlabs.ai
  spf: true
hosts:
- cert_expires: Sep 29 06:24:29 2026 GMT
  host: priorlabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 16:42:38 2026 GMT
  host: api.priorlabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Priorlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prior Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prior Labs
provider_slug: priorlabs
slug: priorlabs-domain-security
source_filename: priorlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: priorlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:24:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.priorlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:42:38 2026 GMT\n  hsts: null\ndomains:\n- domain: priorlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/priorlabs/refs/heads/main/security/priorlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Machine Learning
- Artificial Intelligence
- Tabular Data
- Foundation Models
- Predictions
- Data Science
- MCP
- SDK
---
