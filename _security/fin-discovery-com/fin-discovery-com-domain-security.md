---
api_specs:
- filename: fin-discovery-com-call-tool-api-openapi.yml
  format: yaml
  label: Fintel Discovery Call Tool API
  slug: fin-discovery-com-call-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-call-tool-api-openapi.yml
- filename: fin-discovery-com-fastapi-api-openapi.yml
  format: yaml
  label: Fintel Discovery Fast API
  slug: fin-discovery-com-fastapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-fastapi-api-openapi.yml
- filename: fin-discovery-com-getatoken-api-openapi.yml
  format: yaml
  label: Fintel Discovery Get A Token API
  slug: fin-discovery-com-getatoken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-getatoken-api-openapi.yml
- filename: fin-discovery-com-login-api-openapi.yml
  format: yaml
  label: Fintel Discovery Login API
  slug: fin-discovery-com-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-login-api-openapi.yml
- filename: fin-discovery-com-tool-endpoint-api-openapi.yml
  format: yaml
  label: Fintel Discovery Tool Endpoint API
  slug: fin-discovery-com-tool-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-tool-endpoint-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fin-discovery.com
  spf: true
hosts:
- cert_expires: Dec 31 21:28:13 2026 GMT
  host: fin-discovery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fintel Discovery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fintel Discovery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fintel Discovery
provider_slug: fin-discovery-com
slug: fin-discovery-com-domain-security
source_filename: fin-discovery-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fin-discovery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 21:28:13 2026 GMT\n  hsts: false\ndomains:\n- domain: fin-discovery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fin-discovery-com/security/fin-discovery-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Regulatory Data
- Broker Check
- SEC EDGAR
- Market Data
- MCP Server
- AI Agents
- Compliance
---
