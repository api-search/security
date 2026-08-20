---
api_specs:
- filename: plinth-us-grants-data-analyze-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Analyze API
  slug: plinth-us-grants-data-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-analyze-api-openapi.yml
- filename: plinth-us-grants-data-grants-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Grants API
  slug: plinth-us-grants-data-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-grants-api-openapi.yml
- filename: plinth-us-grants-data-organizations-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Organizations API
  slug: plinth-us-grants-data-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-organizations-api-openapi.yml
- filename: plinth-us-grants-data-resolve-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Resolve API
  slug: plinth-us-grants-data-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-resolve-api-openapi.yml
- filename: plinth-us-grants-data-sql-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data SQL API
  slug: plinth-us-grants-data-sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-sql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: useplinth.com
  spf: true
hosts:
- cert_expires: Sep 14 20:29:22 2026 GMT
  host: data.useplinth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plinth Us Grants Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plinth US Grants Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Plinth US Grants Data
provider_slug: plinth-us-grants-data
slug: plinth-us-grants-data-domain-security
source_filename: plinth-us-grants-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.useplinth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:29:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: useplinth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/security/plinth-us-grants-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Philanthropy
- Grants
- Non-Profit
- Foundations
- IRS 990
- Open Data
- Government Spending
- Research
- Agents
- REST
- JSON
- MCP
- SQL
---
