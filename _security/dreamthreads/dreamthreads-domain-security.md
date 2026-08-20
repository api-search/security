---
api_specs:
- filename: openapi.json
  format: json
  label: DreamGraph API
  slug: dreamgraph-api
  spec_type: OpenAPI
  url: https://mydreamthreads.xyz/dream-interpretation-api/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mydreamthreads.xyz
  spf: false
hosts:
- cert_expires: Oct  4 00:34:43 2026 GMT
  host: mydreamthreads.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dreamthreads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DreamThreads, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: DreamThreads
provider_slug: dreamthreads
slug: dreamthreads-domain-security
source_filename: dreamthreads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mydreamthreads.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 00:34:43 2026 GMT\n  hsts: false\ndomains:\n- domain: mydreamthreads.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamthreads/refs/heads/main/security/dreamthreads-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- dream analysis
- dream interpretation
- Natural Language Processing
- structured parsing
- AI Agents
- MCP Server
- OpenAPI
- wellness / sleep
- research tooling
---
