---
api_specs:
- filename: upscrape-com-pinterest-api-openapi.yml
  format: yaml
  label: upscrape-com Pinterest API
  slug: upscrape-com-pinterest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upscrape-com/openapi/upscrape-com-pinterest-api-openapi.yml
- filename: upscrape-com-system-api-openapi.yml
  format: yaml
  label: upscrape-com System API
  slug: upscrape-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upscrape-com/openapi/upscrape-com-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upscrape.com
  spf: true
hosts:
- cert_expires: Dec  4 16:48:00 2026 GMT
  host: upscrape.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: upscrape-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for upscrape-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: upscrape-com
provider_slug: upscrape-com
slug: upscrape-com-domain-security
source_filename: upscrape-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upscrape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 16:48:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upscrape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/upscrape-com/security/upscrape-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web Scraping
- Data Extraction
- AI Integration
- MCP
---
