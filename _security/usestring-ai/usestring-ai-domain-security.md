---
api_specs:
- filename: usestring-ai-browser-api-openapi.yml
  format: yaml
  label: usestring-ai Browser API
  slug: usestring-ai-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-browser-api-openapi.yml
- filename: usestring-ai-builds-api-openapi.yml
  format: yaml
  label: usestring-ai Builds API
  slug: usestring-ai-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-builds-api-openapi.yml
- filename: usestring-ai-contexts-api-openapi.yml
  format: yaml
  label: usestring-ai Contexts API
  slug: usestring-ai-contexts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-contexts-api-openapi.yml
- filename: usestring-ai-documentation-api-openapi.yml
  format: yaml
  label: usestring-ai Documentation API
  slug: usestring-ai-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-documentation-api-openapi.yml
- filename: usestring-ai-feeds-api-openapi.yml
  format: yaml
  label: usestring-ai Feeds API
  slug: usestring-ai-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-feeds-api-openapi.yml
- filename: usestring-ai-fetch-api-openapi.yml
  format: yaml
  label: usestring-ai Fetch API
  slug: usestring-ai-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-fetch-api-openapi.yml
- filename: usestring-ai-search-api-openapi.yml
  format: yaml
  label: usestring-ai Search API
  slug: usestring-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-search-api-openapi.yml
- filename: usestring-ai-sessions-api-openapi.yml
  format: yaml
  label: usestring-ai Sessions API
  slug: usestring-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-sessions-api-openapi.yml
- filename: usestring-ai-sitemap-api-openapi.yml
  format: yaml
  label: usestring-ai Sitemap API
  slug: usestring-ai-sitemap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-sitemap-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: usestring.ai
  spf: true
hosts:
- cert_expires: Jan 27 23:52:28 2027 GMT
  host: usestring.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: String Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for String, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: String
provider_slug: usestring-ai
slug: usestring-ai-domain-security
source_filename: usestring-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usestring.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:52:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usestring.ai\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/usestring-ai/security/usestring-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web Scraping
- Data Extraction
- Markdown
- JSON
---
