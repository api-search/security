---
api_specs:
- filename: nordpool-market-data-openapi.yml
  format: yaml
  label: Nord Pool Day-Ahead Prices API
  slug: nordpool-day-ahead-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-market-data-openapi.yml
- filename: nordpool-market-data-openapi.yml
  format: yaml
  label: Nord Pool Intraday Market Data API
  slug: nordpool-intraday-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-market-data-openapi.yml
- filename: nordpool-market-data-openapi.yml
  format: yaml
  label: Nord Pool Power System Data API
  slug: nordpool-power-system-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-market-data-openapi.yml
- filename: nordpool-data-portal-openapi.yml
  format: yaml
  label: Nord Pool Public Data Portal API
  slug: nordpool-public-data-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-data-portal-openapi.yml
- filename: nordpool-intraday-asyncapi.yml
  format: yaml
  label: Nord Pool Intraday Trading API
  slug: nordpool-intraday-trading-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/asyncapi/nordpool-intraday-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nordpoolgroup.com
  spf: true
hosts:
- cert_expires: Sep 11 04:29:16 2026 GMT
  host: www.nordpoolgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:03:40 2026 GMT
  host: developers.nordpoolgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 04:29:16 2026 GMT
  host: data-api.nordpoolgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nordpool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nord Pool, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nord Pool
provider_slug: nordpool
slug: nordpool-domain-security
source_filename: nordpool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nordpoolgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:29:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.nordpoolgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:03:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data-api.nordpoolgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:29:16 2026 GMT\n  hsts: null\ndomains:\n- domain: nordpoolgroup.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/security/nordpool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Day-Ahead Prices
- Electricity
- Energy Markets
- Power Exchange
- Intraday Trading
- Market Data
- Europe
---
