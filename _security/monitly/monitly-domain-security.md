---
api_specs:
- filename: monitly-charts-api-openapi.yml
  format: yaml
  label: Monitly Charts API
  slug: monitly-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monitly/refs/heads/main/openapi/monitly-charts-api-openapi.yml
- filename: monitly-datasets-api-openapi.yml
  format: yaml
  label: Monitly Datasets API
  slug: monitly-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monitly/refs/heads/main/openapi/monitly-datasets-api-openapi.yml
- filename: monitly-mcp-api-openapi.yml
  format: yaml
  label: Monitly MCP API
  slug: monitly-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monitly/refs/heads/main/openapi/monitly-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monit.ly
  spf: true
hosts:
- cert_expires: Dec 31 17:09:19 2026 GMT
  host: monit.ly
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Monitly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monitly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Monitly
provider_slug: monitly
slug: monitly-domain-security
source_filename: monitly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monit.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 17:09:19 2026 GMT\n  hsts: false\ndomains:\n- domain: monit.ly\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monitly/refs/heads/main/security/monitly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Statistics
- Dashboards
---
