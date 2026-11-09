---
api_specs:
- filename: birdsift-com-auth-api-openapi.yml
  format: yaml
  label: BirdSift Auth API
  slug: birdsift-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdsift-com/openapi/birdsift-com-auth-api-openapi.yml
- filename: birdsift-com-credits-api-openapi.yml
  format: yaml
  label: BirdSift Credits API
  slug: birdsift-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdsift-com/openapi/birdsift-com-credits-api-openapi.yml
- filename: birdsift-com-docs-api-openapi.yml
  format: yaml
  label: BirdSift Docs API
  slug: birdsift-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdsift-com/openapi/birdsift-com-docs-api-openapi.yml
- filename: birdsift-com-leads-api-openapi.yml
  format: yaml
  label: BirdSift Leads API
  slug: birdsift-com-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdsift-com/openapi/birdsift-com-leads-api-openapi.yml
- filename: birdsift-com-mcp-api-openapi.yml
  format: yaml
  label: BirdSift MCP API
  slug: birdsift-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdsift-com/openapi/birdsift-com-mcp-api-openapi.yml
- filename: birdsift-com-searches-api-openapi.yml
  format: yaml
  label: BirdSift Searches API
  slug: birdsift-com-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdsift-com/openapi/birdsift-com-searches-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: birdsift.com
  spf: true
hosts:
- cert_expires: Dec  9 16:42:23 2026 GMT
  host: birdsift.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Birdsift Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BirdSift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BirdSift
provider_slug: birdsift-com
slug: birdsift-com-domain-security
source_filename: birdsift-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: birdsift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 16:42:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: birdsift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/birdsift-com/security/birdsift-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Lead Generation
- Web Design
- Software-as-a-Service
- Marketing
---
