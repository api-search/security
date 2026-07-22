---
api_specs:
- filename: replicas-openapi-original.json
  format: json
  label: Replica API
  slug: replica-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tryreplicas.com
  spf: true
hosts:
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.tryreplicas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Replicas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Replicas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Replicas
provider_slug: replicas
slug: replicas-domain-security
source_filename: replicas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.tryreplicas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tryreplicas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/security/replicas-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Coding Agents
- Developer Tools
- Automation
- Cloud Workspaces
- MCP
- DevOps
---
