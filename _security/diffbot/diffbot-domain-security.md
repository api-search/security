---
api_specs:
- filename: diffbot-extract-openapi.json
  format: json
  label: Diffbot Extract API
  slug: diffbot-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-extract-openapi.json
- filename: diffbot-crawl-openapi.json
  format: json
  label: Diffbot Crawl API
  slug: diffbot-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-crawl-openapi.json
- filename: diffbot-bulk-openapi.json
  format: json
  label: Diffbot Bulk Extract API
  slug: diffbot-bulk-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-bulk-openapi.json
- filename: diffbot-dql-openapi.json
  format: json
  label: Diffbot DQL API
  slug: diffbot-dql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-dql-openapi.json
- filename: diffbot-enhance-openapi.json
  format: json
  label: Diffbot Enhance API
  slug: diffbot-enhance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-enhance-openapi.json
- filename: diffbot-natural-language-openapi.json
  format: json
  label: Diffbot Natural Language API
  slug: diffbot-natural-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-natural-language-openapi.json
- filename: diffbot-web-search-openapi.json
  format: json
  label: Diffbot Web Search API
  slug: diffbot-web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-web-search-openapi.json
- filename: diffbot-account-openapi.json
  format: json
  label: Diffbot Account API
  slug: diffbot-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-account-openapi.json
- filename: diffbot-knowledge-graph-api-openapi.yml
  format: yaml
  label: Diffbot Knowledge Graph API
  slug: diffbot-knowledge-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/diffbot-knowledge-graph-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diffbot.com
  spf: true
hosts:
- cert_expires: Nov  1 15:52:43 2026 GMT
  host: www.diffbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 09:06:01 2026 GMT
  host: docs.diffbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 05:40:32 2026 GMT
  host: api.diffbot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Diffbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diffbot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diffbot
provider_slug: diffbot
slug: diffbot-domain-security
source_filename: diffbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diffbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:52:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.diffbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 09:06:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.diffbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 05:40:32 2026 GMT\n  hsts: null\ndomains:\n- domain: diffbot.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/security/diffbot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Extraction
- Harvesting
- Scraping
- Web
- Knowledge Graph
- Crawling
- Web Search
- Natural Language
- Entity Resolution
- AI
---
