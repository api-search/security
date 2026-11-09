---
api_specs:
- filename: aihot-news-agent-api-openapi.yml
  format: yaml
  label: AIHOT Agent API
  slug: aihot-news-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-agent-api-openapi.yml
- filename: aihot-news-dailies-api-openapi.yml
  format: yaml
  label: AIHOT Dailies API
  slug: aihot-news-dailies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-dailies-api-openapi.yml
- filename: aihot-news-hot-topics-api-openapi.yml
  format: yaml
  label: AIHOT Hot Topics API
  slug: aihot-news-hot-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-hot-topics-api-openapi.yml
- filename: aihot-news-items-api-openapi.yml
  format: yaml
  label: AIHOT Items API
  slug: aihot-news-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-items-api-openapi.yml
- filename: aihot-news-monthlies-api-openapi.yml
  format: yaml
  label: AIHOT Monthlies API
  slug: aihot-news-monthlies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-monthlies-api-openapi.yml
- filename: aihot-news-selected-api-openapi.yml
  format: yaml
  label: AIHOT Selected API
  slug: aihot-news-selected-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-selected-api-openapi.yml
- filename: aihot-news-stories-api-openapi.yml
  format: yaml
  label: AIHOT Stories API
  slug: aihot-news-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-stories-api-openapi.yml
- filename: aihot-news-weeklies-api-openapi.yml
  format: yaml
  label: AIHOT Weeklies API
  slug: aihot-news-weeklies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-weeklies-api-openapi.yml
description: ''
domains:
- caa:
  - aihot.news.eo.dnse2.com.
  dmarc: false
  dnssec: true
  domain: aihot.news
  spf: false
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: aihot.news
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aihot News Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIHOT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: AIHOT
provider_slug: aihot-news
slug: aihot-news-domain-security
source_filename: aihot-news-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aihot.news\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aihot.news\n  dnssec: true\n  caa:\n  - aihot.news.eo.dnse2.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aihot-news/security/aihot-news-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
---
