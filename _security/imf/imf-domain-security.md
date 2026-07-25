---
api_specs:
- filename: imf-data-api-openapi.yml
  format: yaml
  label: IMF Data Data API
  slug: imf-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imf/refs/heads/main/openapi/imf-data-api-openapi.yml
- filename: imf-structure-api-openapi.yml
  format: yaml
  label: IMF Data Structure API
  slug: imf-structure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imf/refs/heads/main/openapi/imf-structure-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imf.org
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.imf.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: data.imf.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.imf.org
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Imf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IMF Data, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IMF Data
provider_slug: imf
slug: imf-domain-security
source_filename: imf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.imf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: data.imf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: api.imf.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: imf.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imf/refs/heads/main/security/imf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Data
- Economic Indicators
- Balance of Payments
- Exchange Rates
- International Finance
- SDMX
- Macroeconomics
- Fiscal Policy
- Monetary Statistics
- Government Finance
---
