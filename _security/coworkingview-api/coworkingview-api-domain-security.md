---
api_specs:
- filename: coworkingview-api-config-api-openapi.yml
  format: yaml
  label: CoworkingView API Config API
  slug: coworkingview-api-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-config-api-openapi.yml
- filename: coworkingview-api-facets-api-openapi.yml
  format: yaml
  label: CoworkingView API Facets API
  slug: coworkingview-api-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-facets-api-openapi.yml
- filename: coworkingview-api-geo-api-openapi.yml
  format: yaml
  label: CoworkingView API Geo API
  slug: coworkingview-api-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-geo-api-openapi.yml
- filename: coworkingview-api-health-api-openapi.yml
  format: yaml
  label: CoworkingView API Health API
  slug: coworkingview-api-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-health-api-openapi.yml
- filename: coworkingview-api-leads-api-openapi.yml
  format: yaml
  label: CoworkingView API Leads API
  slug: coworkingview-api-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-leads-api-openapi.yml
- filename: coworkingview-api-market-api-openapi.yml
  format: yaml
  label: CoworkingView API Market API
  slug: coworkingview-api-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-market-api-openapi.yml
- filename: coworkingview-api-operators-api-openapi.yml
  format: yaml
  label: CoworkingView API Operators API
  slug: coworkingview-api-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-operators-api-openapi.yml
- filename: coworkingview-api-places-api-openapi.yml
  format: yaml
  label: CoworkingView API Places API
  slug: coworkingview-api-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-places-api-openapi.yml
- filename: coworkingview-api-properties-api-openapi.yml
  format: yaml
  label: CoworkingView API Properties API
  slug: coworkingview-api-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-properties-api-openapi.yml
- filename: coworkingview-api-rankings-api-openapi.yml
  format: yaml
  label: CoworkingView API Rankings API
  slug: coworkingview-api-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-rankings-api-openapi.yml
- filename: coworkingview-api-search-api-openapi.yml
  format: yaml
  label: CoworkingView API Search API
  slug: coworkingview-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: coworkingview.com
  spf: true
hosts:
- cert_expires: Oct 30 06:47:31 2026 GMT
  host: coworkingview.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 06:47:31 2026 GMT
  host: api.coworkingview.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 06:47:31 2026 GMT
  host: mcp.coworkingview.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Coworkingview Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoworkingView API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CoworkingView API
provider_slug: coworkingview-api
slug: coworkingview-api-domain-security
source_filename: coworkingview-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coworkingview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 06:47:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coworkingview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 06:47:31 2026 GMT\n  hsts: null\n- host: mcp.coworkingview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 06:47:31 2026 GMT\n  hsts: false\ndomains:\n- domain: coworkingview.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/security/coworkingview-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Co-Working
- Flexible Workspace
- Real-Estate
- Location Services
- Search
- Comparison
- MCP
- agent-native
- Business
---
