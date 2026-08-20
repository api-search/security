---
api_specs:
- filename: commodity-futures-trading-commission-cot-api-openapi.yml
  format: yaml
  label: Commodity Futures Trading Commission COT API
  slug: commodity-futures-trading-commission-cot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/openapi/commodity-futures-trading-commission-cot-api-openapi.yml
- filename: commodity-futures-trading-commission-disaggregated-api-openapi.yml
  format: yaml
  label: Commodity Futures Trading Commission Disaggregated API
  slug: commodity-futures-trading-commission-disaggregated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/openapi/commodity-futures-trading-commission-disaggregated-api-openapi.yml
- filename: commodity-futures-trading-commission-legacy-api-openapi.yml
  format: yaml
  label: Commodity Futures Trading Commission Legacy API
  slug: commodity-futures-trading-commission-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/openapi/commodity-futures-trading-commission-legacy-api-openapi.yml
- filename: commodity-futures-trading-commission-supplemental-api-openapi.yml
  format: yaml
  label: Commodity Futures Trading Commission Supplemental API
  slug: commodity-futures-trading-commission-supplemental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/openapi/commodity-futures-trading-commission-supplemental-api-openapi.yml
- filename: commodity-futures-trading-commission-tff-api-openapi.yml
  format: yaml
  label: Commodity Futures Trading Commission TFF API
  slug: commodity-futures-trading-commission-tff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/openapi/commodity-futures-trading-commission-tff-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cftc.gov
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.cftc.gov
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 02:51:28 2027 GMT
  host: publicreporting.cftc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Commodity Futures Trading Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commodity Futures Trading Commission, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Commodity Futures Trading Commission
provider_slug: commodity-futures-trading-commission
slug: commodity-futures-trading-commission-domain-security
source_filename: commodity-futures-trading-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cftc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: publicreporting.cftc.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 19 02:51:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cftc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/security/commodity-futures-trading-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CFTC
- Commitments of Traders
- Federal-Government
- Financial
- Futures
- Open Data
- SODA
- Trading
---
