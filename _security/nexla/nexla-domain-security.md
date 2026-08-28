---
api_specs:
- filename: nexla-rest-api-openapi.yml
  format: yaml
  label: Nexla REST API
  slug: nexla-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/openapi/nexla-rest-api-openapi.yml
- filename: nexla-genai-mcpaas-openapi.json
  format: json
  label: Nexla GenAI API (RAG + MCPaaS)
  slug: nexla-genai-api-rag-mcpaas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/openapi/nexla-genai-mcpaas-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nexla.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nexla.io
  spf: true
hosts:
- cert_expires: Nov 20 04:09:39 2026 GMT
  host: nexla.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 16:34:25 2026 GMT
  host: docs.nexla.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: dataops.nexla.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api-genai.nexla.io
  hsts: false
  https: true
  note: Nexla GenAI / MCPaaS host — serves the public OpenAPI and the remote MCP endpoint. No HSTS.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexla, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nexla
provider_slug: nexla
slug: nexla-domain-security
source_filename: nexla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 04:09:39 2026 GMT\n  hsts: false\n- host: docs.nexla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 16:34:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dataops.nexla.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-genai.nexla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n  note: Nexla GenAI / MCPaaS host — serves the public OpenAPI and the remote MCP endpoint. No HSTS.\ndomains:\n- domain: nexla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nexla.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nnotes: 'Probed 2026-08-26 across every apis.yml baseURL\
  \ host plus the docs host. Findings worth acting\n  on: nexla.com serves NO HSTS header, and api-genai.nexla.io — the host that serves the remote MCP endpoint\n  agents authenticate to with a permanent service key — serves no HSTS either. Neither nexla.com nor nexla.io\n  publishes a CAA record or has DNSSEC enabled. nexla.io has SPF but NO DMARC record at all, while nexla.com\n  has DMARC at p=quarantine.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/security/nexla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Integration
- Data Engineering
- ETL
- ELT
- Data Products
- Streaming
- Change Data Capture
- Data Governance
- Artificial Intelligence
- Retrieval Augmented Generation
- MCP
- Agent Tools
- Data Pipelines
- Connectors
---
