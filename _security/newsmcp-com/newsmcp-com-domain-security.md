---
api_specs:
- filename: newsmcp-com-health-api-openapi.yml
  format: yaml
  label: NewsMCP Health API
  slug: newsmcp-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/newsmcp-com/openapi/newsmcp-com-health-api-openapi.yml
- filename: newsmcp-com-limits-api-openapi.yml
  format: yaml
  label: NewsMCP Limits API
  slug: newsmcp-com-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/newsmcp-com/openapi/newsmcp-com-limits-api-openapi.yml
- filename: newsmcp-com-news-api-openapi.yml
  format: yaml
  label: NewsMCP News API
  slug: newsmcp-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/newsmcp-com/openapi/newsmcp-com-news-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: newsmcp.com
  spf: false
hosts:
- cert_expires: Jan  4 15:31:17 2027 GMT
  host: newsmcp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NewsMCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NewsMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NewsMCP
provider_slug: newsmcp-com
slug: newsmcp-com-domain-security
source_filename: newsmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newsmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 15:31:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: newsmcp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/newsmcp-com/security/newsmcp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- News
- Artificial Intelligence
- News API
- MCP
- Aggregation
---
