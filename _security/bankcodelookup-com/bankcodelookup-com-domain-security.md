---
api_specs:
- filename: bankcodelookup-com-dataset-api-openapi.yml
  format: yaml
  label: Bank Code Lookup Dataset API
  slug: bankcodelookup-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankcodelookup-com/openapi/bankcodelookup-com-dataset-api-openapi.yml
- filename: bankcodelookup-com-enquiry-api-openapi.yml
  format: yaml
  label: Bank Code Lookup Enquiry API
  slug: bankcodelookup-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankcodelookup-com/openapi/bankcodelookup-com-enquiry-api-openapi.yml
- filename: bankcodelookup-com-mcp-api-openapi.yml
  format: yaml
  label: Bank Code Lookup MCP API
  slug: bankcodelookup-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankcodelookup-com/openapi/bankcodelookup-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bankcodelookup.com
  spf: true
hosts:
- cert_expires: Dec 10 06:59:13 2026 GMT
  host: bankcodelookup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bank Code Lookup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank Code Lookup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bank Code Lookup
provider_slug: bankcodelookup-com
slug: bankcodelookup-com-domain-security
source_filename: bankcodelookup-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bankcodelookup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bankcodelookup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bankcodelookup-com/security/bankcodelookup-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Banking
- Finance
- Lookup
- Codes
---
