---
api_specs:
- filename: curtilo-com-dataset-api-openapi.yml
  format: yaml
  label: Curtilo Dataset API
  slug: curtilo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curtilo-com/openapi/curtilo-com-dataset-api-openapi.yml
- filename: curtilo-com-mcp-api-openapi.yml
  format: yaml
  label: Curtilo MCP API
  slug: curtilo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curtilo-com/openapi/curtilo-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: curtilo.com
  spf: true
hosts:
- cert_expires: Feb  1 14:58:11 2027 GMT
  host: curtilo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curtilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curtilo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Curtilo
provider_slug: curtilo-com
slug: curtilo-com-domain-security
source_filename: curtilo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curtilo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 14:58:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curtilo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/curtilo-com/security/curtilo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Planning
- Permitted Development
- Property Development
- Land Sourcing
- Real Estate
- United Kingdom
- Datasets
---
