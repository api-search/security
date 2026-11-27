---
api_specs:
- filename: contracko-com-authentication-api-openapi.yml
  format: yaml
  label: Contracko Authentication API
  slug: contracko-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-authentication-api-openapi.yml
- filename: contracko-com-contract-types-api-openapi.yml
  format: yaml
  label: Contracko Contract Types API
  slug: contracko-com-contract-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-contract-types-api-openapi.yml
- filename: contracko-com-parsing-api-api-openapi.yml
  format: yaml
  label: Contracko Parsing API
  slug: contracko-com-parsing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-parsing-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: contracko.com
  spf: true
hosts:
- cert_expires: Jan 23 14:53:43 2027 GMT
  host: contracko.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contracko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contracko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Contracko
provider_slug: contracko-com
slug: contracko-com-domain-security
source_filename: contracko-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contracko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 14:53:43 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: contracko.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/contracko-com/security/contracko-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Contract Management
- Legal Tech
- Artificial Intelligence
- Document Parsing
- Data Extraction
- E-Signature
- MCP
---
