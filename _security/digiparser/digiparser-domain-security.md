---
api_specs:
- filename: digiparser-document-processing-api-openapi.yml
  format: yaml
  label: DigiParser Document processing API
  slug: digiparser-document-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digiparser/openapi/digiparser-document-processing-api-openapi.yml
- filename: digiparser-mcp-api-openapi.yml
  format: yaml
  label: DigiParser MCP API
  slug: digiparser-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digiparser/openapi/digiparser-mcp-api-openapi.yml
- filename: digiparser-parsers-api-openapi.yml
  format: yaml
  label: DigiParser Parsers API
  slug: digiparser-parsers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digiparser/openapi/digiparser-parsers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: digiparser.com
  spf: false
hosts:
- cert_expires: Dec 18 09:13:49 2026 GMT
  host: www.digiparser.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digiparser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigiParser, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: DigiParser
provider_slug: digiparser
slug: digiparser-domain-security
source_filename: digiparser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digiparser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 09:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: digiparser.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/digiparser/security/digiparser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Document-Processing
- API
- Automation
- Data-Extraction
- AI
---
