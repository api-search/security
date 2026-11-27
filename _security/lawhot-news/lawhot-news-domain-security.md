---
api_specs:
- filename: lawhot-news-agent-api-openapi.yml
  format: yaml
  label: LAWHOT Agent API
  slug: lawhot-news-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawhot-news/openapi/lawhot-news-agent-api-openapi.yml
- filename: lawhot-news-dailies-api-openapi.yml
  format: yaml
  label: LAWHOT Dailies API
  slug: lawhot-news-dailies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawhot-news/openapi/lawhot-news-dailies-api-openapi.yml
- filename: lawhot-news-hot-topics-api-openapi.yml
  format: yaml
  label: LAWHOT Hot Topics API
  slug: lawhot-news-hot-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawhot-news/openapi/lawhot-news-hot-topics-api-openapi.yml
- filename: lawhot-news-items-api-openapi.yml
  format: yaml
  label: LAWHOT Items API
  slug: lawhot-news-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawhot-news/openapi/lawhot-news-items-api-openapi.yml
- filename: lawhot-news-monthlies-api-openapi.yml
  format: yaml
  label: LAWHOT Monthlies API
  slug: lawhot-news-monthlies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawhot-news/openapi/lawhot-news-monthlies-api-openapi.yml
- filename: lawhot-news-selected-api-openapi.yml
  format: yaml
  label: LAWHOT Selected API
  slug: lawhot-news-selected-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawhot-news/openapi/lawhot-news-selected-api-openapi.yml
- filename: lawhot-news-stories-api-openapi.yml
  format: yaml
  label: LAWHOT Stories API
  slug: lawhot-news-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawhot-news/openapi/lawhot-news-stories-api-openapi.yml
- filename: lawhot-news-weeklies-api-openapi.yml
  format: yaml
  label: LAWHOT Weeklies API
  slug: lawhot-news-weeklies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawhot-news/openapi/lawhot-news-weeklies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lawhot.news
  spf: false
hosts:
- cert_expires: Feb  6 21:46:09 2027 GMT
  host: lawhot.news
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LAWHOT Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LAWHOT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LAWHOT
provider_slug: lawhot-news
slug: lawhot-news-domain-security
source_filename: lawhot-news-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lawhot.news\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 21:46:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lawhot.news\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lawhot-news/security/lawhot-news-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Legal
- News
- Aggregation
- Daily Digest
---
