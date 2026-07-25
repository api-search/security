---
api_specs:
- filename: apify-actor-runs-api-openapi.yml
  format: yaml
  label: Apify Actor Runs API
  slug: apify-actor-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/openapi/apify-actor-runs-api-openapi.yml
- filename: apify-actors-api-openapi.yml
  format: yaml
  label: Apify Actors API
  slug: apify-actors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/openapi/apify-actors-api-openapi.yml
- filename: apify-datasets-api-openapi.yml
  format: yaml
  label: Apify Datasets API
  slug: apify-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/openapi/apify-datasets-api-openapi.yml
- filename: apify-key-value-stores-api-openapi.yml
  format: yaml
  label: Apify Key-Value Stores API
  slug: apify-key-value-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/openapi/apify-key-value-stores-api-openapi.yml
- filename: apify-request-queues-api-openapi.yml
  format: yaml
  label: Apify Request Queues API
  slug: apify-request-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/openapi/apify-request-queues-api-openapi.yml
- filename: apify-users-api-openapi.yml
  format: yaml
  label: Apify Users API
  slug: apify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/openapi/apify-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: apify.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: apify.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.apify.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Apify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Apify
provider_slug: apify
slug: apify-domain-security
source_filename: apify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.apify.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: apify.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/security/apify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Actors
- Browser Automation
- Crawling
- Data Aggregation
- Data Extraction
- Web Automation
- Web Scraping
---
