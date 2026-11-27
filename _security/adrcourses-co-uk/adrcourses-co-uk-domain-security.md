---
api_specs:
- filename: adrcourses-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: ADR Courses Enquiry API
  slug: adrcourses-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adrcourses-co-uk/openapi/adrcourses-co-uk-enquiry-api-openapi.yml
- filename: adrcourses-co-uk-mcp-api-openapi.yml
  format: yaml
  label: ADR Courses MCP API
  slug: adrcourses-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adrcourses-co-uk/openapi/adrcourses-co-uk-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adrcourses.co.uk
  spf: true
hosts:
- cert_expires: Jan  9 23:20:42 2027 GMT
  host: adrcourses.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ADR Courses Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADR Courses, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ADR Courses
provider_slug: adrcourses-co-uk
slug: adrcourses-co-uk-domain-security
source_filename: adrcourses-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adrcourses.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:20:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adrcourses.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/adrcourses-co-uk/security/adrcourses-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ADR
- Training
- United Kingdom
- Transportation
- Safety
---
