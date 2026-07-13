---
api_specs:
- filename: import-io-openapi.yml
  format: yaml
  label: Import.io API
  slug: import-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/import-io/main/openapi/import-io-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: import.io
  spf: true
hosts:
- cert_expires: Sep  2 10:33:58 2026 GMT
  host: www.import.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.import.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Import Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Import.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Import.io
provider_slug: import-io
slug: import-io-domain-security
source_filename: import-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.import.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 10:33:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.import.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: import.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/import-io/refs/heads/main/security/import-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Aggregation
- Data Extraction
- Data Integration
- Pricing Intelligence
- Web Scraping
---
