---
api_specs:
- filename: clauselane-com-dataset-api-openapi.yml
  format: yaml
  label: clauselane-com Dataset API
  slug: clauselane-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clauselane-com/openapi/clauselane-com-dataset-api-openapi.yml
- filename: clauselane-com-mcp-api-openapi.yml
  format: yaml
  label: clauselane-com MCP API
  slug: clauselane-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clauselane-com/openapi/clauselane-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clauselane.com
  spf: true
hosts:
- cert_expires: Dec  4 04:26:07 2026 GMT
  host: clauselane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clauselane Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for clauselane-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: clauselane-com
provider_slug: clauselane-com
slug: clauselane-com-domain-security
source_filename: clauselane-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clauselane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 04:26:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clauselane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/clauselane-com/security/clauselane-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- LegalTech
- ContractManagement
- SaaS
- SmallBusiness
- US
---
