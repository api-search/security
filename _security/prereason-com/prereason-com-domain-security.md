---
api_specs:
- filename: prereason-com-agent-access-api-openapi.yml
  format: yaml
  label: prereason-com Agent access API
  slug: prereason-com-agent-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-agent-access-api-openapi.yml
- filename: prereason-com-company-briefings-api-openapi.yml
  format: yaml
  label: prereason-com Company Briefings API
  slug: prereason-com-company-briefings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-company-briefings-api-openapi.yml
- filename: prereason-com-context-api-openapi.yml
  format: yaml
  label: prereason-com Context API
  slug: prereason-com-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-context-api-openapi.yml
- filename: prereason-com-metrics-api-openapi.yml
  format: yaml
  label: prereason-com Metrics API
  slug: prereason-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-metrics-api-openapi.yml
- filename: prereason-com-short-urls-api-openapi.yml
  format: yaml
  label: prereason-com Short URLs API
  slug: prereason-com-short-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-short-urls-api-openapi.yml
- filename: prereason-com-system-api-openapi.yml
  format: yaml
  label: prereason-com System API
  slug: prereason-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-system-api-openapi.yml
- filename: prereason-com-treasury-holdings-api-openapi.yml
  format: yaml
  label: prereason-com Treasury Holdings API
  slug: prereason-com-treasury-holdings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-treasury-holdings-api-openapi.yml
- filename: prereason-com-webhooks-api-openapi.yml
  format: yaml
  label: prereason-com Webhooks API
  slug: prereason-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prereason.com
  spf: true
hosts:
- cert_expires: Dec 26 08:29:53 2026 GMT
  host: prereason.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prereason Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for prereason-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: prereason-com
provider_slug: prereason-com
slug: prereason-com-domain-security
source_filename: prereason-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prereason.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 08:29:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prereason.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/prereason-com/security/prereason-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Market
- API
- AI
- Data
- MCP
---
