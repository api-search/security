---
api_specs:
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Latest Rates API
  slug: latest-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Pair Conversion API
  slug: pair-conversion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Enriched Data API
  slug: enriched-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Historical Rates API
  slug: historical-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Supported Codes API
  slug: supported-codes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Quota API
  slug: quota
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Open Access API
  slug: open-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exchangerate-api.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: er-api.com
  spf: true
hosts:
- cert_expires: Sep 14 15:00:24 2026 GMT
  host: www.exchangerate-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:00:24 2026 GMT
  host: v6.exchangerate-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 03:05:42 2026 GMT
  host: open.er-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exchangerate Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExchangeRate-API, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ExchangeRate-API
provider_slug: exchangerate-api
slug: exchangerate-api-domain-security
source_filename: exchangerate-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exchangerate-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:00:24 2026 GMT\n  hsts: false\n- host: v6.exchangerate-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:00:24 2026 GMT\n  hsts: false\n- host: open.er-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:05:42 2026 GMT\n  hsts: false\ndomains:\n- domain: exchangerate-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: er-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/security/exchangerate-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency Exchange
- Foreign Exchange
- Financial Data
- Forex
- Currency Conversion
- Public APIs
---
