---
api_specs:
- filename: clubgrants-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Club Grants Enquiry API
  slug: clubgrants-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clubgrants-co-uk/openapi/clubgrants-co-uk-enquiry-api-openapi.yml
- filename: clubgrants-co-uk-guide-api-openapi.yml
  format: yaml
  label: Club Grants Guide API
  slug: clubgrants-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clubgrants-co-uk/openapi/clubgrants-co-uk-guide-api-openapi.yml
- filename: clubgrants-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Club Grants MCP API
  slug: clubgrants-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clubgrants-co-uk/openapi/clubgrants-co-uk-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clubgrants.co.uk
  spf: true
hosts:
- cert_expires: Jan 10 01:59:50 2027 GMT
  host: clubgrants.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Club Grants Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Club Grants, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Club Grants
provider_slug: clubgrants-co-uk
slug: clubgrants-co-uk-domain-security
source_filename: clubgrants-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clubgrants.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:59:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clubgrants.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/clubgrants-co-uk/security/clubgrants-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Grants
- Funding
- Sports
- Non-Profit
- Open Data
- United Kingdom
- MCP
---
