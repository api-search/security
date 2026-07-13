---
api_specs:
- filename: restack-openapi.yml
  format: yaml
  label: Restack
  slug: restack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restack/refs/heads/main/openapi/restack-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: restack.io
  spf: true
hosts:
- cert_expires: Aug 23 17:31:14 2026 GMT
  host: www.restack.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.restack.io
  https: false
kind: domain-security
layout: security
method: probed
name: Restack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Restack, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Restack
provider_slug: restack
slug: restack-domain-security
source_filename: restack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.restack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 17:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.restack.io\n  https: false\ndomains:\n- domain: restack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restack/refs/heads/main/security/restack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Workflows
- Orchestration
- Enterprise
- Python
---
