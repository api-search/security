---
api_specs:
- filename: aladdin-studio-analytics-api-openapi.yml
  format: yaml
  label: Aladdin Studio Analytics API
  slug: aladdin-studio-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-analytics-api-openapi.yml
- filename: aladdin-studio-connections-api-openapi.yml
  format: yaml
  label: Aladdin Studio Connections API
  slug: aladdin-studio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-connections-api-openapi.yml
- filename: aladdin-studio-datasets-api-openapi.yml
  format: yaml
  label: Aladdin Studio Datasets API
  slug: aladdin-studio-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-datasets-api-openapi.yml
- filename: aladdin-studio-orders-api-openapi.yml
  format: yaml
  label: Aladdin Studio Orders API
  slug: aladdin-studio-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-orders-api-openapi.yml
- filename: aladdin-studio-portfolios-api-openapi.yml
  format: yaml
  label: Aladdin Studio Portfolios API
  slug: aladdin-studio-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-portfolios-api-openapi.yml
- filename: aladdin-studio-positions-api-openapi.yml
  format: yaml
  label: Aladdin Studio Positions API
  slug: aladdin-studio-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-positions-api-openapi.yml
- filename: aladdin-studio-queries-api-openapi.yml
  format: yaml
  label: Aladdin Studio Queries API
  slug: aladdin-studio-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-queries-api-openapi.yml
- filename: aladdin-studio-research-api-openapi.yml
  format: yaml
  label: Aladdin Studio Research API
  slug: aladdin-studio-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-research-api-openapi.yml
- filename: aladdin-studio-risk-api-openapi.yml
  format: yaml
  label: Aladdin Studio Risk API
  slug: aladdin-studio-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-risk-api-openapi.yml
- filename: aladdin-studio-securities-api-openapi.yml
  format: yaml
  label: Aladdin Studio Securities API
  slug: aladdin-studio-securities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-securities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blackrock.com
  spf: true
hosts:
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: www.blackrock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: api.blackrock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aladdin Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aladdin Studio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aladdin Studio
provider_slug: aladdin-studio
slug: aladdin-studio-domain-security
source_filename: aladdin-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blackrock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.blackrock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: blackrock.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/security/aladdin-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
---
