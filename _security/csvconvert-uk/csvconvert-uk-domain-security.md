---
api_specs:
- filename: csvconvert-uk-enquiry-api-openapi.yml
  format: yaml
  label: CSV Convert Enquiry API
  slug: csvconvert-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csvconvert-uk/openapi/csvconvert-uk-enquiry-api-openapi.yml
- filename: csvconvert-uk-guide-api-openapi.yml
  format: yaml
  label: CSV Convert Guide API
  slug: csvconvert-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csvconvert-uk/openapi/csvconvert-uk-guide-api-openapi.yml
- filename: csvconvert-uk-mcp-api-openapi.yml
  format: yaml
  label: CSV Convert MCP API
  slug: csvconvert-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csvconvert-uk/openapi/csvconvert-uk-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: csvconvert.uk
  spf: true
hosts:
- cert_expires: Jan  9 21:16:53 2027 GMT
  host: csvconvert.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CSV Convert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CSV Convert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CSV Convert
provider_slug: csvconvert-uk
slug: csvconvert-uk-domain-security
source_filename: csvconvert-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: csvconvert.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 21:16:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: csvconvert.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/csvconvert-uk/security/csvconvert-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CSV
- PDF
- Data Conversion
- Data Extraction
- OCR
- United Kingdom
- Data Protection
---
