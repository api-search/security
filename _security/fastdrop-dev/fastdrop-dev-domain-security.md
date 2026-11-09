---
api_specs:
- filename: fastdrop-dev-health-api-openapi.yml
  format: yaml
  label: FastDrop Health API
  slug: fastdrop-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-health-api-openapi.yml
- filename: fastdrop-dev-mcp-api-openapi.yml
  format: yaml
  label: FastDrop MCP API
  slug: fastdrop-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-mcp-api-openapi.yml
- filename: fastdrop-dev-subregistry-api-openapi.yml
  format: yaml
  label: FastDrop Subregistry API
  slug: fastdrop-dev-subregistry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-subregistry-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fastdrop.dev
  spf: true
hosts:
- cert_expires: Dec 17 11:05:54 2026 GMT
  host: fastdrop.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fastdrop Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FastDrop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FastDrop
provider_slug: fastdrop-dev
slug: fastdrop-dev-domain-security
source_filename: fastdrop-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastdrop.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 11:05:54 2026 GMT\n  hsts: false\ndomains:\n- domain: fastdrop.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fastdrop-dev/security/fastdrop-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- launch-board
- MCP
- AI-agents
- software-discovery
- free-service
---
