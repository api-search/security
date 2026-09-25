---
api_specs:
- filename: browser-use-billing-api-openapi.yml
  format: yaml
  label: Browser Use Billing API
  slug: browser-use-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-billing-api-openapi.yml
- filename: browser-use-browsers-api-openapi.yml
  format: yaml
  label: Browser Use Browsers API
  slug: browser-use-browsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-browsers-api-openapi.yml
- filename: browser-use-files-api-openapi.yml
  format: yaml
  label: Browser Use Files API
  slug: browser-use-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-files-api-openapi.yml
- filename: browser-use-profiles-api-openapi.yml
  format: yaml
  label: Browser Use Profiles API
  slug: browser-use-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-profiles-api-openapi.yml
- filename: browser-use-runs-api-openapi.yml
  format: yaml
  label: Browser Use Runs API
  slug: browser-use-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-runs-api-openapi.yml
- filename: browser-use-sessions-api-openapi.yml
  format: yaml
  label: Browser Use Sessions API
  slug: browser-use-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-sessions-api-openapi.yml
- filename: browser-use-skills-api-openapi.yml
  format: yaml
  label: Browser Use Skills API
  slug: browser-use-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-skills-api-openapi.yml
- filename: browser-use-skills-marketplace-api-openapi.yml
  format: yaml
  label: Browser Use Skills Marketplace API
  slug: browser-use-skills-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-skills-marketplace-api-openapi.yml
- filename: browser-use-tasks-api-openapi.yml
  format: yaml
  label: Browser Use Tasks API
  slug: browser-use-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-tasks-api-openapi.yml
- filename: browser-use-workspaces-api-openapi.yml
  format: yaml
  label: Browser Use Workspaces API
  slug: browser-use-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-workspaces-api-openapi.yml
- filename: browser-use-x402-api-openapi.yml
  format: yaml
  label: Browser Use X402 API
  slug: browser-use-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: browser-use.com
  spf: true
hosts:
- cert_expires: Oct 27 06:22:02 2026 GMT
  host: browser-use.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 21:16:21 2026 GMT
  host: docs.browser-use.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.browser-use.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Browser Use Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Browser Use, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Browser Use
provider_slug: browser-use
slug: browser-use-domain-security
source_filename: browser-use-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: browser-use.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 06:22:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.browser-use.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:16:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.browser-use.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: browser-use.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/security/browser-use-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Automation
- Browser Automation
- Web Agents
- Web Scraping
- Headless Browser
- Agent Infrastructure
- MCP
- Cloud Browsers
- A2A
---
