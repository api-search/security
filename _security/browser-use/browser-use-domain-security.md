---
api_specs:
- filename: browser-use-api-v4-openapi.json
  format: json
  label: Browser Use Public API v4
  slug: browser-use-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v4-openapi.json
- filename: browser-use-api-v3-openapi.json
  format: json
  label: Browser Use Public API v3
  slug: browser-use-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v3-openapi.json
- filename: browser-use-api-v2-openapi.json
  format: json
  label: Browser Use Public API v2
  slug: browser-use-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v2-openapi.json
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
- Headless Browsers
- Agent Infrastructure
- MCP
- Cloud Browsers
---
