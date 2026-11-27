---
api_specs:
- filename: ffpipe-dev-discovery-api-openapi.yml
  format: yaml
  label: ffpipe Discovery API
  slug: ffpipe-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffpipe-dev/openapi/ffpipe-dev-discovery-api-openapi.yml
- filename: ffpipe-dev-feedback-api-openapi.yml
  format: yaml
  label: ffpipe Feedback API
  slug: ffpipe-dev-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffpipe-dev/openapi/ffpipe-dev-feedback-api-openapi.yml
- filename: ffpipe-dev-jobs-api-openapi.yml
  format: yaml
  label: ffpipe Jobs API
  slug: ffpipe-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffpipe-dev/openapi/ffpipe-dev-jobs-api-openapi.yml
- filename: ffpipe-dev-mcp-api-openapi.yml
  format: yaml
  label: ffpipe MCP API
  slug: ffpipe-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffpipe-dev/openapi/ffpipe-dev-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ffpipe.dev
  spf: false
hosts:
- cert_expires: Jan  9 23:18:27 2027 GMT
  host: ffpipe.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ffpipe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ffpipe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ffpipe
provider_slug: ffpipe-dev
slug: ffpipe-dev-domain-security
source_filename: ffpipe-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ffpipe.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:18:27 2027 GMT\n  hsts: false\ndomains:\n- domain: ffpipe.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ffpipe-dev/security/ffpipe-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Media
- Payments
- Video
- Automation
---
