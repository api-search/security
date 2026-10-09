---
api_specs:
- filename: datacircle-datacircle-api-openapi.yml
  format: yaml
  label: Datacircle Datacircle API
  slug: datacircle-datacircle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-datacircle-api-openapi.yml
- filename: datacircle-harvestapi-api-openapi.yml
  format: yaml
  label: Datacircle Harvest API
  slug: datacircle-harvestapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-harvestapi-api-openapi.yml
- filename: datacircle-up2data-api-openapi.yml
  format: yaml
  label: Datacircle Up2 Data API
  slug: datacircle-up2data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-up2data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datacircle.dev
  spf: true
hosts:
- cert_expires: Jan  5 02:45:21 2027 GMT
  host: datacircle.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datacircle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datacircle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datacircle
provider_slug: datacircle
slug: datacircle-domain-security
source_filename: datacircle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datacircle.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 02:45:21 2027 GMT\n  hsts: false\ndomains:\n- domain: datacircle.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/security/datacircle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- B2B Data
- Data Enrichment
- LinkedIn
- Profiles
- MCP
- Data Co-op
---
