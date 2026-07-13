---
api_specs:
- filename: firecrawl-openapi-original.json
  format: json
  label: Firecrawl API
  slug: firecrawl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firecrawl/refs/heads/main/openapi/firecrawl-openapi-original.json
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
