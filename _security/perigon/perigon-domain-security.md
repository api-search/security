---
api_specs:
- filename: perigon-ai-advanced-search-api-openapi.yml
  format: yaml
  label: Perigon AI & Advanced Search API
  slug: perigon-ai-advanced-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-ai-advanced-search-api-openapi.yml
- filename: perigon-contact-points-api-openapi.yml
  format: yaml
  label: Perigon Contact Points API
  slug: perigon-contact-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-contact-points-api-openapi.yml
- filename: perigon-monitors-api-openapi.yml
  format: yaml
  label: Perigon Monitors API
  slug: perigon-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-monitors-api-openapi.yml
- filename: perigon-news-stories-api-openapi.yml
  format: yaml
  label: Perigon News & Stories API
  slug: perigon-news-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-news-stories-api-openapi.yml
- filename: perigon-source-groups-api-openapi.yml
  format: yaml
  label: Perigon Source Groups API
  slug: perigon-source-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-source-groups-api-openapi.yml
- filename: perigon-supplemental-endpoints-api-openapi.yml
  format: yaml
  label: Perigon Supplemental Endpoints API
  slug: perigon-supplemental-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-supplemental-endpoints-api-openapi.yml
- filename: perigon-utilities-api-openapi.yml
  format: yaml
  label: Perigon Utilities API
  slug: perigon-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-utilities-api-openapi.yml
- filename: perigon-watchlists-api-openapi.yml
  format: yaml
  label: Perigon Watchlists API
  slug: perigon-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-watchlists-api-openapi.yml
- filename: perigon-wikipedia-api-openapi.yml
  format: yaml
  label: Perigon Wikipedia API
  slug: perigon-wikipedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-wikipedia-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "0 issue \"amazon.com\""
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: perigon.io
  spf: true
hosts:
- cert_expires: Nov 22 11:16:45 2026 GMT
  host: perigon.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Perigon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perigon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Perigon
provider_slug: perigon
slug: perigon-domain-security
source_filename: perigon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perigon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 11:16:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: perigon.io\n  dnssec: true\n  caa:\n  - 0 issue \"0 issue \\\"amazon.com\\\"\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/security/perigon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- News
- Media Monitoring
- Search
- Artificial Intelligence
- Data
- MCP
- Webhook
---
