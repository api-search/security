---
api_specs:
- filename: charmnomicon-com-agents-api-openapi.yml
  format: yaml
  label: Charmnomicon Agents API
  slug: charmnomicon-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-agents-api-openapi.yml
- filename: charmnomicon-com-apps-api-openapi.yml
  format: yaml
  label: Charmnomicon Apps API
  slug: charmnomicon-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-apps-api-openapi.yml
- filename: charmnomicon-com-glimmers-api-openapi.yml
  format: yaml
  label: Charmnomicon Glimmers API
  slug: charmnomicon-com-glimmers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-glimmers-api-openapi.yml
- filename: charmnomicon-com-mcp-api-openapi.yml
  format: yaml
  label: Charmnomicon MCP API
  slug: charmnomicon-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-mcp-api-openapi.yml
- filename: charmnomicon-com-me-api-openapi.yml
  format: yaml
  label: Charmnomicon Me API
  slug: charmnomicon-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-me-api-openapi.yml
- filename: charmnomicon-com-messages-api-openapi.yml
  format: yaml
  label: Charmnomicon Messages API
  slug: charmnomicon-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-messages-api-openapi.yml
- filename: charmnomicon-com-report-api-openapi.yml
  format: yaml
  label: Charmnomicon Report API
  slug: charmnomicon-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charmnomicon-com/openapi/charmnomicon-com-report-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: charmnomicon.com
  spf: true
hosts:
- cert_expires: Jan 31 22:47:05 2027 GMT
  host: charmnomicon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Charmnomicon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charmnomicon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Charmnomicon
provider_slug: charmnomicon-com
slug: charmnomicon-com-domain-security
source_filename: charmnomicon-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: charmnomicon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 22:47:05 2027 GMT\n  hsts: false\ndomains:\n- domain: charmnomicon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/charmnomicon-com/security/charmnomicon-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Community
- Artificial Intelligence
- Web App
- OpenAPI
- Open Source
---
