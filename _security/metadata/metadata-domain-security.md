---
api_specs:
- filename: metadata-health-api-openapi.yml
  format: yaml
  label: Metadata Health API
  slug: metadata-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metadata/refs/heads/main/openapi/metadata-health-api-openapi.yml
- filename: metadata-mcp-api-openapi.yml
  format: yaml
  label: Metadata MCP API
  slug: metadata-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metadata/refs/heads/main/openapi/metadata-mcp-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metadata.io
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: metadata.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: mcp-server.metadata.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metadata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metadata, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metadata
provider_slug: metadata
slug: metadata-domain-security
source_filename: metadata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metadata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: mcp-server.metadata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: metadata.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metadata/refs/heads/main/security/metadata-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- Marketing Automation
- Demand Generation
- Advertising
- B2B
- Artificial Intelligence
- MCP
- AI Agents
- Paid Media
- Account Based Marketing
---
