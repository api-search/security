---
api_specs:
- filename: apex-new-openapi-generated.yml
  format: yaml
  label: Apex by LeadShark API
  slug: apex-new-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apex-new/openapi/_ae-authored/apex-new-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apex.new
  spf: true
hosts:
- cert_expires: Jan 27 06:05:46 2027 GMT
  host: www.apex.new
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apex New Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apex by LeadShark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Apex by LeadShark
provider_slug: apex-new
slug: apex-new-domain-security
source_filename: apex-new-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apex.new\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 06:05:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apex.new\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/apex-new/security/apex-new-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- LinkedIn
- Artificial Intelligence
- Automation
- Lead Generation
- MCP
---
