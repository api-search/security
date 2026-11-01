---
api_specs:
- filename: unplain-io-discovery-api-openapi.yml
  format: yaml
  label: unplain-io Discovery API
  slug: unplain-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unplain-io/openapi/unplain-io-discovery-api-openapi.yml
- filename: unplain-io-feature-requests-api-openapi.yml
  format: yaml
  label: unplain-io Feature requests API
  slug: unplain-io-feature-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unplain-io/openapi/unplain-io-feature-requests-api-openapi.yml
- filename: unplain-io-mcp-api-openapi.yml
  format: yaml
  label: unplain-io MCP API
  slug: unplain-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unplain-io/openapi/unplain-io-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unplain.io
  spf: true
hosts:
- cert_expires: Jan 18 16:04:57 2027 GMT
  host: unplain.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unplain Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for unplain-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: unplain-io
provider_slug: unplain-io
slug: unplain-io-domain-security
source_filename: unplain-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unplain.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 16:04:57 2027 GMT\n  hsts: false\ndomains:\n- domain: unplain.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/unplain-io/security/unplain-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- PDF
- AI
- Marketing
- SaaS
---
