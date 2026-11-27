---
api_specs:
- filename: nessgate-com-connect-api-openapi.yml
  format: yaml
  label: NessGate Connect API
  slug: nessgate-com-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessgate-com/openapi/nessgate-com-connect-api-openapi.yml
- filename: nessgate-com-discover-api-openapi.yml
  format: yaml
  label: NessGate Discover API
  slug: nessgate-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessgate-com/openapi/nessgate-com-discover-api-openapi.yml
- filename: nessgate-com-explore-api-openapi.yml
  format: yaml
  label: NessGate Explore API
  slug: nessgate-com-explore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessgate-com/openapi/nessgate-com-explore-api-openapi.yml
- filename: nessgate-com-mcp-api-openapi.yml
  format: yaml
  label: NessGate MCP API
  slug: nessgate-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessgate-com/openapi/nessgate-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nessgate.com
  spf: true
hosts:
- cert_expires: Feb  4 01:53:18 2027 GMT
  host: nessgate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NessGate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NessGate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: NessGate
provider_slug: nessgate-com
slug: nessgate-com-domain-security
source_filename: nessgate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nessgate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 01:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nessgate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nessgate-com/security/nessgate-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Resolver
- Agentic Web
- Open Source
- Neutral
---
