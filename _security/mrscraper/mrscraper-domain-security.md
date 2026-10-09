---
api_specs:
- filename: mrscraper-analytic-api-openapi.yml
  format: yaml
  label: MrScraper Analytic API
  slug: mrscraper-analytic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-analytic-api-openapi.yml
- filename: mrscraper-auth-api-openapi.yml
  format: yaml
  label: MrScraper Auth API
  slug: mrscraper-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-auth-api-openapi.yml
- filename: mrscraper-gateway-api-openapi.yml
  format: yaml
  label: MrScraper Gateway API
  slug: mrscraper-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-gateway-api-openapi.yml
- filename: mrscraper-jobs-api-openapi.yml
  format: yaml
  label: MrScraper Jobs API
  slug: mrscraper-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-jobs-api-openapi.yml
- filename: mrscraper-proxies-api-openapi.yml
  format: yaml
  label: MrScraper Proxies API
  slug: mrscraper-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-proxies-api-openapi.yml
- filename: mrscraper-results-api-openapi.yml
  format: yaml
  label: MrScraper Results API
  slug: mrscraper-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-results-api-openapi.yml
- filename: mrscraper-storage-api-openapi.yml
  format: yaml
  label: MrScraper Storage API
  slug: mrscraper-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-storage-api-openapi.yml
- filename: mrscraper-tasks-api-openapi.yml
  format: yaml
  label: MrScraper Tasks API
  slug: mrscraper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-tasks-api-openapi.yml
description: ''
domains:
- caa:
  - mrscraper.b-cdn.net.
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mrscraper.com
  spf: true
hosts:
- cert_expires: Dec 31 06:06:03 2026 GMT
  host: mrscraper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mrscraper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MrScraper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MrScraper
provider_slug: mrscraper
slug: mrscraper-domain-security
source_filename: mrscraper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mrscraper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 06:06:03 2026 GMT\n  hsts: false\ndomains:\n- domain: mrscraper.com\n  dnssec: true\n  caa:\n  - mrscraper.b-cdn.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/security/mrscraper-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Web Scraping
- Data Extraction
- Proxies
- AI Agents
- MCP
- Search
- Browser Automation
---
