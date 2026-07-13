---
api_specs:
- filename: kontomatik-ais-api-openapi.yml
  format: yaml
  label: Kontomatik Account Information Service API
  slug: kontomatik-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-ais-api-openapi.yml
- filename: kontomatik-pdf-parsing-api-openapi.yml
  format: yaml
  label: Kontomatik PDF Parsing API
  slug: kontomatik-pdf-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-pdf-parsing-api-openapi.yml
- filename: kontomatik-data-analysis-api-openapi.yml
  format: yaml
  label: Kontomatik Data Analysis API
  slug: kontomatik-data-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-data-analysis-api-openapi.yml
- filename: kontomatik-report-api-openapi.yml
  format: yaml
  label: Kontomatik Report API
  slug: kontomatik-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-report-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kontomatik.com
  spf: true
hosts:
- cert_expires: Oct  8 15:52:18 2026 GMT
  host: kontomatik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 03:01:18 2026 GMT
  host: developer.kontomatik.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 18:39:22 2026 GMT
  host: api.kontomatik.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kontomatik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kontomatik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kontomatik
provider_slug: kontomatik
slug: kontomatik-domain-security
source_filename: kontomatik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kontomatik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:52:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.kontomatik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:01:18 2026 GMT\n  hsts: false\n- host: api.kontomatik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:39:22 2026 GMT\n  hsts: null\ndomains:\n- domain: kontomatik.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/security/kontomatik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Banking
- PSD2
- AIS
- Bank Data Aggregation
- CEE
- KYC
- Credit Scoring
- Transaction Labeling
- PDF Parsing
---
