---
api_specs:
- filename: meilisearch-documents-api-openapi.yml
  format: yaml
  label: Meilisearch Documents API
  slug: meilisearch-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-documents-api-openapi.yml
- filename: meilisearch-health-api-openapi.yml
  format: yaml
  label: Meilisearch Health API
  slug: meilisearch-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-health-api-openapi.yml
- filename: meilisearch-indexes-api-openapi.yml
  format: yaml
  label: Meilisearch Indexes API
  slug: meilisearch-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-indexes-api-openapi.yml
- filename: meilisearch-keys-api-openapi.yml
  format: yaml
  label: Meilisearch Keys API
  slug: meilisearch-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-keys-api-openapi.yml
- filename: meilisearch-search-api-openapi.yml
  format: yaml
  label: Meilisearch Search API
  slug: meilisearch-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-search-api-openapi.yml
- filename: meilisearch-settings-api-openapi.yml
  format: yaml
  label: Meilisearch Settings API
  slug: meilisearch-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-settings-api-openapi.yml
- filename: meilisearch-tasks-api-openapi.yml
  format: yaml
  label: Meilisearch Tasks API
  slug: meilisearch-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-tasks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: meilisearch.com
  spf: true
hosts:
- cert_expires: Sep 17 06:22:12 2026 GMT
  host: www.meilisearch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meilisearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meilisearch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Meilisearch
provider_slug: meilisearch
slug: meilisearch-domain-security
source_filename: meilisearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meilisearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:22:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: meilisearch.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/security/meilisearch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Search
- Full-Text Search
- Hybrid Search
- Open-Source
- Search
---
