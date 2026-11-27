---
api_specs:
- filename: deflectvo-com-dataset-api-openapi.yml
  format: yaml
  label: Deflectvo Dataset API
  slug: deflectvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deflectvo-com/openapi/deflectvo-com-dataset-api-openapi.yml
- filename: deflectvo-com-mcp-api-openapi.yml
  format: yaml
  label: Deflectvo MCP API
  slug: deflectvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deflectvo-com/openapi/deflectvo-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deflectvo.com
  spf: true
hosts:
- cert_expires: Jan 31 18:33:12 2027 GMT
  host: deflectvo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deflectvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deflectvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Deflectvo
provider_slug: deflectvo-com
slug: deflectvo-com-domain-security
source_filename: deflectvo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deflectvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 18:33:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deflectvo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/deflectvo-com/security/deflectvo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Customer Self-Service
- Customer Service
- Help Center
- Ticket Deflection
- Customer Portal
- Software-as-a-Service
---
