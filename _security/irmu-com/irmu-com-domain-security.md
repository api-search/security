---
api_specs:
- filename: irmu-com-booking-api-openapi.yml
  format: yaml
  label: Irmu Booking API
  slug: irmu-com-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-booking-api-openapi.yml
- filename: irmu-com-crawl-api-openapi.yml
  format: yaml
  label: Irmu Crawl API
  slug: irmu-com-crawl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-crawl-api-openapi.yml
- filename: irmu-com-google-api-openapi.yml
  format: yaml
  label: Irmu Google API
  slug: irmu-com-google-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-google-api-openapi.yml
- filename: irmu-com-screenshot-api-openapi.yml
  format: yaml
  label: Irmu Screenshot API
  slug: irmu-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-screenshot-api-openapi.yml
- filename: irmu-com-chat-gpt-api-openapi.yml
  format: yaml
  label: Irmu Chat GPT API
  slug: irmu-com-chat-gpt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-chat-gpt-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: irmu.com
  spf: true
hosts:
- cert_expires: Jan 23 18:31:12 2027 GMT
  host: irmu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Irmu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Irmu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Irmu
provider_slug: irmu-com
slug: irmu-com-domain-security
source_filename: irmu-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: irmu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 18:31:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: irmu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/irmu-com/security/irmu-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Scraping
- Developer Tools
- Automation
- Data Extraction
- Company
---
