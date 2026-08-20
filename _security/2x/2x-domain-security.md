---
api_specs:
- filename: 2x-knownwell-openapi.json
  format: json
  label: Knownwell Commercial Intelligence API
  slug: knownwell-commercial-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-knownwell-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 2x.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knownwell.com
  spf: true
hosts:
- cert_expires: Oct  1 04:35:42 2026 GMT
  host: 2x.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 16:33:25 2026 GMT
  host: api.knownwell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 22:54:27 2026 GMT
  host: mcp.knownwell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 2X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2X, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 2X
provider_slug: 2x
slug: 2x-domain-security
source_filename: 2x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 2x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:35:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.knownwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 16:33:25 2026 GMT\n  hsts: null\n- host: mcp.knownwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:54:27 2026 GMT\n  hsts: null\ndomains:\n- domain: 2x.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: knownwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/security/2x-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Marketing as a Service
- B2B
- MarTech
- Marketing Operations
- Consulting
- Artificial Intelligence
- Go-To-Market
- Revenue Operations
- Commercial Intelligence
- Customer Success
- Agentic AI
- Demand Generation
---
