---
api_specs:
- filename: packrift-com-ai-api-openapi.yml
  format: yaml
  label: Packrift AI API
  slug: packrift-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packrift-com/openapi/packrift-com-ai-api-openapi.yml
- filename: packrift-com-health-api-openapi.yml
  format: yaml
  label: Packrift Health API
  slug: packrift-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packrift-com/openapi/packrift-com-health-api-openapi.yml
- filename: packrift-com-manifest-api-openapi.yml
  format: yaml
  label: Packrift Manifest API
  slug: packrift-com-manifest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packrift-com/openapi/packrift-com-manifest-api-openapi.yml
- filename: packrift-com-mcp-api-openapi.yml
  format: yaml
  label: Packrift MCP API
  slug: packrift-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packrift-com/openapi/packrift-com-mcp-api-openapi.yml
- filename: packrift-com-products-api-openapi.yml
  format: yaml
  label: Packrift Products API
  slug: packrift-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packrift-com/openapi/packrift-com-products-api-openapi.yml
- filename: packrift-com-r-api-openapi.yml
  format: yaml
  label: Packrift R API
  slug: packrift-com-r-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packrift-com/openapi/packrift-com-r-api-openapi.yml
- filename: packrift-com-resources-api-openapi.yml
  format: yaml
  label: Packrift Resources API
  slug: packrift-com-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packrift-com/openapi/packrift-com-resources-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: packrift.com
  spf: true
hosts:
- cert_expires: Dec 27 18:35:33 2026 GMT
  host: packrift.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Packrift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packrift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Packrift
provider_slug: packrift-com
slug: packrift-com-domain-security
source_filename: packrift-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packrift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 18:35:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: packrift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/packrift-com/security/packrift-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Packaging
- E-Commerce
- Supply Chain
- Warehouse
- Shipping
---
