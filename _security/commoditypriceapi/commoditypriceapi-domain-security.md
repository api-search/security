---
api_specs:
- filename: commoditypriceapi-commoditypriceapi-api-api-openapi.yml
  format: yaml
  label: CommodityPriceAPI CommodityPriceAPI API
  slug: commoditypriceapi-commoditypriceapi-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commoditypriceapi/refs/heads/main/openapi/commoditypriceapi-commoditypriceapi-api-api-openapi.yml
- filename: commoditypriceapi-rates-api-openapi.yml
  format: yaml
  label: CommodityPriceAPI Rates API
  slug: commoditypriceapi-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commoditypriceapi/refs/heads/main/openapi/commoditypriceapi-rates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: commoditypriceapi.com
  spf: true
hosts:
- cert_expires: Dec 11 23:06:23 2026 GMT
  host: commoditypriceapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Commoditypriceapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CommodityPriceAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: CommodityPriceAPI
provider_slug: commoditypriceapi
slug: commoditypriceapi-domain-security
source_filename: commoditypriceapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commoditypriceapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:06:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: commoditypriceapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commoditypriceapi/refs/heads/main/security/commoditypriceapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Commodities
- Finance
- Real-Time
---
