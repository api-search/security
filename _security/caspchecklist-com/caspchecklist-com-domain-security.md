---
api_specs:
- filename: caspchecklist-com-enquiry-api-openapi.yml
  format: yaml
  label: CASP Checklist Enquiry API
  slug: caspchecklist-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspchecklist-com/openapi/caspchecklist-com-enquiry-api-openapi.yml
- filename: caspchecklist-com-guide-api-openapi.yml
  format: yaml
  label: CASP Checklist Guide API
  slug: caspchecklist-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspchecklist-com/openapi/caspchecklist-com-guide-api-openapi.yml
- filename: caspchecklist-com-mcp-api-openapi.yml
  format: yaml
  label: CASP Checklist MCP API
  slug: caspchecklist-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspchecklist-com/openapi/caspchecklist-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: caspchecklist.com
  spf: true
hosts:
- cert_expires: Jan  9 21:11:13 2027 GMT
  host: caspchecklist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CASP Checklist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CASP Checklist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CASP Checklist
provider_slug: caspchecklist-com
slug: caspchecklist-com-domain-security
source_filename: caspchecklist-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caspchecklist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 21:11:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: caspchecklist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/caspchecklist-com/security/caspchecklist-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- EU
- MiCA
- Compliance
---
