---
api_specs:
- filename: firecrawl-account-api-openapi.yml
  format: yaml
  label: Firecrawl Account API
  slug: firecrawl-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-account-api-openapi.yml
- filename: firecrawl-agent-api-openapi.yml
  format: yaml
  label: Firecrawl Agent API
  slug: firecrawl-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-agent-api-openapi.yml
- filename: firecrawl-billing-api-openapi.yml
  format: yaml
  label: Firecrawl Billing API
  slug: firecrawl-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-billing-api-openapi.yml
- filename: firecrawl-browser-api-openapi.yml
  format: yaml
  label: Firecrawl Browser API
  slug: firecrawl-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-browser-api-openapi.yml
- filename: firecrawl-crawling-api-openapi.yml
  format: yaml
  label: Firecrawl Crawling API
  slug: firecrawl-crawling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-crawling-api-openapi.yml
- filename: firecrawl-extraction-api-openapi.yml
  format: yaml
  label: Firecrawl Extraction API
  slug: firecrawl-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-extraction-api-openapi.yml
- filename: firecrawl-mapping-api-openapi.yml
  format: yaml
  label: Firecrawl Mapping API
  slug: firecrawl-mapping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-mapping-api-openapi.yml
- filename: firecrawl-miscellaneous-api-openapi.yml
  format: yaml
  label: Firecrawl Miscellaneous API
  slug: firecrawl-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-miscellaneous-api-openapi.yml
- filename: firecrawl-scraping-api-openapi.yml
  format: yaml
  label: Firecrawl Scraping API
  slug: firecrawl-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-scraping-api-openapi.yml
- filename: firecrawl-search-api-openapi.yml
  format: yaml
  label: Firecrawl Search API
  slug: firecrawl-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firecrawl.dev
  spf: true
hosts:
- cert_expires: Sep 26 07:15:35 2026 GMT
  host: www.firecrawl.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 15:35:03 2026 GMT
  host: docs.firecrawl.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 16:26:41 2026 GMT
  host: api.firecrawl.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firecrawl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firecrawl, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Firecrawl
provider_slug: firecrawl
slug: firecrawl-domain-security
source_filename: firecrawl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firecrawl.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:15:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.firecrawl.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 15:35:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.firecrawl.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:26:41 2026 GMT\n  hsts: false\ndomains:\n- domain: firecrawl.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/security/firecrawl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crawling
- Data Extraction
- Scraping
- URLs
- AI
- Markdown
---
