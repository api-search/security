---
api_specs:
- filename: tinyfish-automation-api-openapi.yml
  format: yaml
  label: TinyFish Automation API
  slug: tinyfish-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-automation-api-openapi.yml
- filename: tinyfish-runs-api-openapi.yml
  format: yaml
  label: TinyFish Runs API
  slug: tinyfish-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-runs-api-openapi.yml
- filename: tinyfish-tinyfish-browser-api-api-openapi.yml
  format: yaml
  label: TinyFish TinyFish Browser API API
  slug: tinyfish-tinyfish-browser-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-tinyfish-browser-api-api-openapi.yml
- filename: tinyfish-tinyfish-fetch-api-api-openapi.yml
  format: yaml
  label: TinyFish TinyFish Fetch API API
  slug: tinyfish-tinyfish-fetch-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-tinyfish-fetch-api-api-openapi.yml
- filename: tinyfish-tinyfish-search-api-api-openapi.yml
  format: yaml
  label: TinyFish TinyFish Search API API
  slug: tinyfish-tinyfish-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-tinyfish-search-api-api-openapi.yml
- filename: tinyfish-usage-api-openapi.yml
  format: yaml
  label: TinyFish Usage API
  slug: tinyfish-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-usage-api-openapi.yml
- filename: tinyfish-vault-api-openapi.yml
  format: yaml
  label: TinyFish Vault API
  slug: tinyfish-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-vault-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tinyfish.ai
  spf: true
hosts:
- cert_expires: Sep 20 17:36:27 2026 GMT
  host: www.tinyfish.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.browser.tinyfish.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.fetch.tinyfish.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tinyfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TinyFish, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TinyFish
provider_slug: tinyfish
slug: tinyfish-domain-security
source_filename: tinyfish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tinyfish.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:36:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.browser.tinyfish.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: api.fetch.tinyfish.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tinyfish.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/security/tinyfish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- AI Agents
- Web Automation
- Web Scraping
- Search
- Browser Automation
- Model Context Protocol
- Data Extraction
---
