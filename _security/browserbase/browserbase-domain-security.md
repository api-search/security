---
api_specs:
- filename: browserbase-contexts-api-openapi.yml
  format: yaml
  label: Browserbase Contexts API
  slug: browserbase-contexts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-contexts-api-openapi.yml
- filename: browserbase-extensions-api-openapi.yml
  format: yaml
  label: Browserbase Extensions API
  slug: browserbase-extensions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-extensions-api-openapi.yml
- filename: browserbase-projects-api-openapi.yml
  format: yaml
  label: Browserbase Projects API
  slug: browserbase-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-projects-api-openapi.yml
- filename: browserbase-sessions-api-openapi.yml
  format: yaml
  label: Browserbase Sessions API
  slug: browserbase-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-sessions-api-openapi.yml
- filename: browserbase-agents-api-openapi.yml
  format: yaml
  label: Browserbase Agents API
  slug: browserbase-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-agents-api-openapi.yml
- filename: browserbase-certificates-api-openapi.yml
  format: yaml
  label: Browserbase Certificates API
  slug: browserbase-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-certificates-api-openapi.yml
- filename: browserbase-downloads-api-openapi.yml
  format: yaml
  label: Browserbase Downloads API
  slug: browserbase-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-downloads-api-openapi.yml
- filename: browserbase-fetch-api-openapi.yml
  format: yaml
  label: Browserbase Fetch API
  slug: browserbase-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-fetch-api-openapi.yml
- filename: browserbase-functions-api-openapi.yml
  format: yaml
  label: Browserbase Functions API
  slug: browserbase-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-functions-api-openapi.yml
- filename: browserbase-search-api-openapi.yml
  format: yaml
  label: Browserbase Search API
  slug: browserbase-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-search-api-openapi.yml
- filename: browserbase-secrets-api-openapi.yml
  format: yaml
  label: Browserbase Secrets API
  slug: browserbase-secrets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-secrets-api-openapi.yml
- filename: browserbase-webhooks-api-openapi.yml
  format: yaml
  label: Browserbase Webhooks API
  slug: browserbase-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: browserbase.com
  spf: true
hosts:
- cert_expires: Aug 21 20:38:31 2026 GMT
  host: www.browserbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 09:01:35 2026 GMT
  host: docs.browserbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: api.browserbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Browserbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Browserbase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Browserbase
provider_slug: browserbase
slug: browserbase-domain-security
source_filename: browserbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.browserbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 20:38:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.browserbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 09:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.browserbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: browserbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/browserbase/security/browserbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser Automation
- Browser Infrastructure
- AI Agents
- Web Scraping
- Stagehand
- Playwright
- Puppeteer
- Web Search
- Web Fetch
- Model Gateway
- MCP
- Session Recording
- Agent Identity
---
