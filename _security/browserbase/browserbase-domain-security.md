---
api_specs:
- filename: browserbase-openapi.yml
  format: yaml
  label: Browserbase API
  slug: browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserbase/refs/heads/main/openapi/browserbase-openapi.yml
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browserbase/refs/heads/main/security/browserbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Headless Browser
- Browser Infrastructure
- Web Automation
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
