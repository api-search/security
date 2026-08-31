---
api_specs:
- filename: botify-analysis-api-openapi.yml
  format: yaml
  label: Botify Analysis API
  slug: botify-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-analysis-api-openapi.yml
- filename: botify-collections-api-openapi.yml
  format: yaml
  label: Botify Collections API
  slug: botify-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-collections-api-openapi.yml
- filename: botify-datasource-api-openapi.yml
  format: yaml
  label: Botify Datasource API
  slug: botify-datasource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-datasource-api-openapi.yml
- filename: botify-job-api-openapi.yml
  format: yaml
  label: Botify Job API
  slug: botify-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-job-api-openapi.yml
- filename: botify-keywordsgroups-api-openapi.yml
  format: yaml
  label: Botify Keywords Groups API
  slug: botify-keywordsgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-keywordsgroups-api-openapi.yml
- filename: botify-project-api-openapi.yml
  format: yaml
  label: Botify Project API
  slug: botify-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-project-api-openapi.yml
- filename: botify-projectquery-api-openapi.yml
  format: yaml
  label: Botify Project Query API
  slug: botify-projectquery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-projectquery-api-openapi.yml
- filename: botify-user-api-openapi.yml
  format: yaml
  label: Botify User API
  slug: botify-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: botify.com
  spf: true
hosts:
- cert_expires: Nov  5 12:18:33 2026 GMT
  host: www.botify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 04:44:26 2026 GMT
  host: developers.botify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.botify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Botify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Botify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Botify
provider_slug: botify
slug: botify-domain-security
source_filename: botify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.botify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 12:18:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.botify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:44:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.botify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: botify.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/security/botify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- Organic search
- search-engine-optimization
- web-crawling
- log-analysis
- search-console
- marketing-analytics
- AI Search
- data-export
- MCP
- agent-native
---
