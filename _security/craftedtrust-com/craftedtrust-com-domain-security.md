---
api_specs:
- filename: craftedtrust-com-mcp-api-openapi.yml
  format: yaml
  label: CraftedTrust MCP API
  slug: craftedtrust-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftedtrust-com/openapi/craftedtrust-com-mcp-api-openapi.yml
- filename: craftedtrust-com-public-api-openapi.yml
  format: yaml
  label: CraftedTrust Public API
  slug: craftedtrust-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftedtrust-com/openapi/craftedtrust-com-public-api-openapi.yml
- filename: craftedtrust-com-publisher-api-openapi.yml
  format: yaml
  label: CraftedTrust Publisher API
  slug: craftedtrust-com-publisher-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftedtrust-com/openapi/craftedtrust-com-publisher-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: craftedtrust.com
  spf: true
hosts:
- cert_expires: Dec  7 04:55:29 2026 GMT
  host: craftedtrust.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CraftedTrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CraftedTrust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CraftedTrust
provider_slug: craftedtrust-com
slug: craftedtrust-com-domain-security
source_filename: craftedtrust-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craftedtrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 04:55:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: craftedtrust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/craftedtrust-com/security/craftedtrust-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- AI Agents
- Security
- Trust Registry
- Security Scanning
---
