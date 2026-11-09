---
api_specs:
- filename: blbestate-com-agent-api-openapi.yml
  format: yaml
  label: SalesSwipe Agent API
  slug: blbestate-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blbestate-com/openapi/blbestate-com-agent-api-openapi.yml
- filename: blbestate-com-mcp-api-openapi.yml
  format: yaml
  label: SalesSwipe MCP API
  slug: blbestate-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blbestate-com/openapi/blbestate-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: blbestate.com
  spf: true
hosts:
- cert_expires: Jan 31 11:46:59 2027 GMT
  host: blbestate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blbestate Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SalesSwipe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SalesSwipe
provider_slug: blbestate-com
slug: blbestate-com-domain-security
source_filename: blbestate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blbestate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 11:46:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blbestate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/blbestate-com/security/blbestate-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- Platform
- Property
- Sales
- Software-as-a-Service
---
