---
api_specs:
- filename: imperioutils-com-demo-pubblica-api-openapi.yml
  format: yaml
  label: Imperio Demo pubblica API
  slug: imperioutils-com-demo-pubblica-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-demo-pubblica-api-openapi.yml
- filename: imperioutils-com-health-api-openapi.yml
  format: yaml
  label: Imperio Health API
  slug: imperioutils-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-health-api-openapi.yml
- filename: imperioutils-com-mcp-api-openapi.yml
  format: yaml
  label: Imperio MCP API
  slug: imperioutils-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-mcp-api-openapi.yml
- filename: imperioutils-com-registry-api-openapi.yml
  format: yaml
  label: Imperio Registry API
  slug: imperioutils-com-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-registry-api-openapi.yml
- filename: imperioutils-com-tool-api-openapi.yml
  format: yaml
  label: Imperio Tool API
  slug: imperioutils-com-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-tool-api-openapi.yml
- filename: imperioutils-com-webhookcapture-api-openapi.yml
  format: yaml
  label: Imperio Webhook Capture API
  slug: imperioutils-com-webhookcapture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-webhookcapture-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imperioutils.com
  spf: true
hosts:
- cert_expires: Jan 11 10:09:27 2027 GMT
  host: imperioutils.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Imperio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imperio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Imperio
provider_slug: imperioutils-com
slug: imperioutils-com-domain-security
source_filename: imperioutils-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imperioutils.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 10:09:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: imperioutils.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/imperioutils-com/security/imperioutils-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Tax
- Fraud Prevention
- Italy
---
