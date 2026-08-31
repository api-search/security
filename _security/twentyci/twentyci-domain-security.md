---
api_specs:
- filename: twentyci-address-match-api-openapi.yml
  format: yaml
  label: TwentyCi Address Match API
  slug: twentyci-address-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-address-match-api-openapi.yml
- filename: twentyci-agent-performance-api-openapi.yml
  format: yaml
  label: TwentyCi Agent Performance API
  slug: twentyci-agent-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-agent-performance-api-openapi.yml
- filename: twentyci-authorisation-api-openapi.yml
  format: yaml
  label: TwentyCi Authorisation API
  slug: twentyci-authorisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-authorisation-api-openapi.yml
- filename: twentyci-categories-api-openapi.yml
  format: yaml
  label: TwentyCi Categories API
  slug: twentyci-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-categories-api-openapi.yml
- filename: twentyci-properties-api-openapi.yml
  format: yaml
  label: TwentyCi Properties API
  slug: twentyci-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-properties-api-openapi.yml
- filename: twentyci-schools-api-openapi.yml
  format: yaml
  label: TwentyCi Schools API
  slug: twentyci-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-schools-api-openapi.yml
- filename: twentyci-this-is-now-retail-propensity-to-buy-goods-api-openapi.yml
  format: yaml
  label: TwentyCi This is Now | Retail Propensity To Buy Goods API
  slug: twentyci-this-is-now-retail-propensity-to-buy-goods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-this-is-now-retail-propensity-to-buy-goods-api-openapi.yml
- filename: twentyci-trigger-information-api-openapi.yml
  format: yaml
  label: TwentyCi Trigger Information API
  slug: twentyci-trigger-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-trigger-information-api-openapi.yml
- filename: twentyci-uk-housing-market-metrics-api-openapi.yml
  format: yaml
  label: TwentyCi UK Housing Market Metrics API
  slug: twentyci-uk-housing-market-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-uk-housing-market-metrics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: twentyci.co.uk
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.twentyci.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.twentyci.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twentyci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TwentyCi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TwentyCi
provider_slug: twentyci
slug: twentyci-domain-security
source_filename: twentyci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twentyci.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.twentyci.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: twentyci.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/security/twentyci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Valuation
- AVM
- Rentals
- Address Data
- Conveyancing
- Homemover Data
- Agent Performance
- Data as a Service
---
