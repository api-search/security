---
api_specs:
- filename: cloro-dev-async-api-openapi.yml
  format: yaml
  label: cloro Async API
  slug: cloro-dev-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-async-api-openapi.yml
- filename: cloro-dev-countries-api-openapi.yml
  format: yaml
  label: cloro Countries API
  slug: cloro-dev-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-countries-api-openapi.yml
- filename: cloro-dev-credits-api-openapi.yml
  format: yaml
  label: cloro Credits API
  slug: cloro-dev-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-credits-api-openapi.yml
- filename: cloro-dev-monitor-api-openapi.yml
  format: yaml
  label: cloro Monitor API
  slug: cloro-dev-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-monitor-api-openapi.yml
- filename: cloro-dev-states-api-openapi.yml
  format: yaml
  label: cloro States API
  slug: cloro-dev-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-states-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cloro.dev
  spf: true
hosts:
- cert_expires: Nov 30 16:17:38 2026 GMT
  host: cloro.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloro Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cloro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: cloro
provider_slug: cloro-dev
slug: cloro-dev-domain-security
source_filename: cloro-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloro.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 16:17:38 2026 GMT\n  hsts: false\ndomains:\n- domain: cloro.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/security/cloro-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Search
- AI
- Web Scraping
- SERP
- Generative Engine Optimization
- SEO
- Brand Monitoring
- Market Research
- Data Extraction
- MCP
---
