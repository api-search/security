---
api_specs:
- filename: catchintent-com-discovery-api-openapi.yml
  format: yaml
  label: CatchIntent Discovery API
  slug: catchintent-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-discovery-api-openapi.yml
- filename: catchintent-com-health-api-openapi.yml
  format: yaml
  label: CatchIntent Health API
  slug: catchintent-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-health-api-openapi.yml
- filename: catchintent-com-mcp-api-openapi.yml
  format: yaml
  label: CatchIntent MCP API
  slug: catchintent-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-mcp-api-openapi.yml
- filename: catchintent-com-oauth-api-openapi.yml
  format: yaml
  label: CatchIntent OAuth API
  slug: catchintent-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-oauth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: catchintent.com
  spf: true
hosts:
- cert_expires: Jan 14 15:03:14 2027 GMT
  host: catchintent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Catchintent Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CatchIntent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CatchIntent
provider_slug: catchintent-com
slug: catchintent-com-domain-security
source_filename: catchintent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catchintent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 15:03:14 2027 GMT\n  hsts: false\ndomains:\n- domain: catchintent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/catchintent-com/security/catchintent-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- B2B
- Sales
- Intent Data
- Artificial Intelligence
- Outbound
---
