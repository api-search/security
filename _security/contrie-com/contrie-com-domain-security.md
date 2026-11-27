---
api_specs:
- filename: contrie-com-account-api-openapi.yml
  format: yaml
  label: Contrie Account API
  slug: contrie-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-account-api-openapi.yml
- filename: contrie-com-evidence-api-openapi.yml
  format: yaml
  label: Contrie Evidence API
  slug: contrie-com-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-evidence-api-openapi.yml
- filename: contrie-com-extract-api-openapi.yml
  format: yaml
  label: Contrie Extract API
  slug: contrie-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-extract-api-openapi.yml
- filename: contrie-com-health-api-openapi.yml
  format: yaml
  label: Contrie Health API
  slug: contrie-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-health-api-openapi.yml
- filename: contrie-com-mcp-api-openapi.yml
  format: yaml
  label: Contrie MCP API
  slug: contrie-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-mcp-api-openapi.yml
- filename: contrie-com-monitors-api-openapi.yml
  format: yaml
  label: Contrie Monitors API
  slug: contrie-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-monitors-api-openapi.yml
- filename: contrie-com-scrape-api-openapi.yml
  format: yaml
  label: Contrie Scrape API
  slug: contrie-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-scrape-api-openapi.yml
- filename: contrie-com-search-api-openapi.yml
  format: yaml
  label: Contrie Search API
  slug: contrie-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-search-api-openapi.yml
- filename: contrie-com-verification-api-openapi.yml
  format: yaml
  label: Contrie Verification API
  slug: contrie-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-verification-api-openapi.yml
- filename: contrie-com-verify-api-openapi.yml
  format: yaml
  label: Contrie Verify API
  slug: contrie-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-verify-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: contrie.com
  spf: true
hosts:
- cert_expires: Dec 16 18:03:10 2026 GMT
  host: contrie.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contrie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contrie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Contrie
provider_slug: contrie-com
slug: contrie-com-domain-security
source_filename: contrie-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contrie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 18:03:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: contrie.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/contrie-com/security/contrie-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Web Scraping
- Data Extraction
- AI Agents
- MCP
- Structured Data
- Markdown
---
