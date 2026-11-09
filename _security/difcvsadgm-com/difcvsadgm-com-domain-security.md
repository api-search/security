---
api_specs:
- filename: difcvsadgm-com-enquiry-api-openapi.yml
  format: yaml
  label: DIFC vs ADGM Enquiry API
  slug: difcvsadgm-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difcvsadgm-com/openapi/difcvsadgm-com-enquiry-api-openapi.yml
- filename: difcvsadgm-com-guide-api-openapi.yml
  format: yaml
  label: DIFC vs ADGM Guide API
  slug: difcvsadgm-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difcvsadgm-com/openapi/difcvsadgm-com-guide-api-openapi.yml
- filename: difcvsadgm-com-mcp-api-openapi.yml
  format: yaml
  label: DIFC vs ADGM MCP API
  slug: difcvsadgm-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difcvsadgm-com/openapi/difcvsadgm-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: difcvsadgm.com
  spf: true
hosts:
- cert_expires: Jan  9 22:20:46 2027 GMT
  host: difcvsadgm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Difcvsadgm Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DIFC vs ADGM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DIFC vs ADGM
provider_slug: difcvsadgm-com
slug: difcvsadgm-com-domain-security
source_filename: difcvsadgm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: difcvsadgm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 22:20:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: difcvsadgm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/difcvsadgm-com/security/difcvsadgm-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Company Formation
- Free Zones
- United Arab Emirates
- Financial Regulation
- Licensing
- MCP
---
