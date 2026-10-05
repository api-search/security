---
api_specs:
- filename: bodo-ai-miniconda-api-openapi.yml
  format: yaml
  label: bodo.ai Miniconda API
  slug: bodo-ai-miniconda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodo-ai/refs/heads/main/openapi/bodo-ai-miniconda-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bodo.ai
  spf: true
hosts:
- cert_expires: Nov  8 17:25:26 2026 GMT
  host: www.bodo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bodo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bodo.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: bodo.ai
provider_slug: bodo-ai
slug: bodo-ai-domain-security
source_filename: bodo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bodo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 17:25:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bodo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodo-ai/refs/heads/main/security/bodo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Artificial Intelligence
- Enterprise
- Open Source
- Data Engineering
---
