---
api_specs:
- filename: apifuse-analytics-api-openapi.yml
  format: yaml
  label: Apifuse Analytics API
  slug: apifuse-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/openapi/apifuse-analytics-api-openapi.yml
- filename: apifuse-connectors-api-openapi.yml
  format: yaml
  label: Apifuse Connectors API
  slug: apifuse-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/openapi/apifuse-connectors-api-openapi.yml
- filename: apifuse-integrations-api-openapi.yml
  format: yaml
  label: Apifuse Integrations API
  slug: apifuse-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/openapi/apifuse-integrations-api-openapi.yml
- filename: apifuse-users-api-openapi.yml
  format: yaml
  label: Apifuse Users API
  slug: apifuse-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/openapi/apifuse-users-api-openapi.yml
- filename: apifuse-workflows-api-openapi.yml
  format: yaml
  label: Apifuse Workflows API
  slug: apifuse-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/openapi/apifuse-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apifuse.io
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: apifuse.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.apifuse.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apifuse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apifuse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apifuse
provider_slug: apifuse
slug: apifuse-domain-security
source_filename: apifuse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apifuse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.apifuse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: apifuse.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/security/apifuse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Embedded Integrations
- Integration Platform
- Integrations
- iPaaS
- Marketplace
- SaaS
- Workflow Automation
---
