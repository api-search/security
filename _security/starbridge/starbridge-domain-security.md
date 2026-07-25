---
api_specs:
- filename: starbridge-bridges-api-openapi.yml
  format: yaml
  label: Starbridge Bridges API
  slug: starbridge-bridges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-bridges-api-openapi.yml
- filename: starbridge-buyer-api-openapi.yml
  format: yaml
  label: Starbridge Buyer API
  slug: starbridge-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-buyer-api-openapi.yml
- filename: starbridge-columns-api-openapi.yml
  format: yaml
  label: Starbridge Columns API
  slug: starbridge-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-columns-api-openapi.yml
- filename: starbridge-external-api-api-openapi.yml
  format: yaml
  label: Starbridge External API API
  slug: starbridge-external-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-external-api-api-openapi.yml
- filename: starbridge-external-mcp-api-openapi.yml
  format: yaml
  label: Starbridge External MCP API
  slug: starbridge-external-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-external-mcp-api-openapi.yml
- filename: starbridge-signal-api-openapi.yml
  format: yaml
  label: Starbridge Signal API
  slug: starbridge-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-signal-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: starbridge.ai
  spf: true
hosts:
- cert_expires: Sep  8 06:36:20 2026 GMT
  host: starbridge.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starbridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starbridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Starbridge
provider_slug: starbridge
slug: starbridge-domain-security
source_filename: starbridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: starbridge.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 06:36:20 2026 GMT\n  hsts: false\ndomains:\n- domain: starbridge.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/security/starbridge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Sales Intelligence
- Go To Market
- Public Sector
- Education
- Government
- Procurement
- Buyer Intelligence
- MCP
---
