---
api_specs:
- filename: regdatalab-com-discovery-api-openapi.yml
  format: yaml
  label: RegDataLab Discovery API
  slug: regdatalab-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regdatalab-com/openapi/regdatalab-com-discovery-api-openapi.yml
- filename: regdatalab-com-mcp-api-openapi.yml
  format: yaml
  label: RegDataLab MCP API
  slug: regdatalab-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regdatalab-com/openapi/regdatalab-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: regdatalab.com
  spf: true
hosts:
- cert_expires: Feb  1 15:02:58 2027 GMT
  host: regdatalab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RegDataLab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RegDataLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RegDataLab
provider_slug: regdatalab-com
slug: regdatalab-com-domain-security
source_filename: regdatalab-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regdatalab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 15:02:58 2027 GMT\n  hsts: null\ndomains:\n- domain: regdatalab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/regdatalab-com/security/regdatalab-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Healthcare
- FDA
- AI
- Chatbot
---
