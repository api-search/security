---
api_specs:
- filename: airtop-ai-query-api-openapi.yml
  format: yaml
  label: Airtop AI Query API
  slug: airtop-ai-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-ai-query-api-openapi.yml
- filename: airtop-page-interaction-api-openapi.yml
  format: yaml
  label: Airtop Page Interaction API
  slug: airtop-page-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-page-interaction-api-openapi.yml
- filename: airtop-profiles-api-openapi.yml
  format: yaml
  label: Airtop Profiles API
  slug: airtop-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-profiles-api-openapi.yml
- filename: airtop-screenshots-api-openapi.yml
  format: yaml
  label: Airtop Screenshots API
  slug: airtop-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-screenshots-api-openapi.yml
- filename: airtop-sessions-api-openapi.yml
  format: yaml
  label: Airtop Sessions API
  slug: airtop-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-sessions-api-openapi.yml
- filename: airtop-windows-api-openapi.yml
  format: yaml
  label: Airtop Windows API
  slug: airtop-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-windows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airtop.ai
  spf: true
hosts:
- cert_expires: Aug  9 20:52:19 2026 GMT
  host: www.airtop.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 16:12:13 2026 GMT
  host: docs.airtop.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.airtop.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airtop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airtop, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airtop
provider_slug: airtop
slug: airtop-domain-security
source_filename: airtop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airtop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 20:52:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.airtop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:12:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.airtop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: airtop.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/security/airtop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser Automation
- AI Agents
- Cloud Browser
- Web Scraping
- Headless Chrome
---
