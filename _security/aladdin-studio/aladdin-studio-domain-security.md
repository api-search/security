---
api_specs:
- filename: aladdin-studio-graph-openapi.yaml
  format: yaml
  label: Aladdin Graph API
  slug: graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-graph-openapi.yaml
- filename: aladdin-studio-data-cloud-openapi.yaml
  format: yaml
  label: Aladdin Data Cloud API
  slug: data-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-data-cloud-openapi.yaml
- filename: aladdin-studio-trading-openapi.yaml
  format: yaml
  label: Aladdin Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-trading-openapi.yaml
- filename: aladdin-studio-investment-research-openapi.yaml
  format: yaml
  label: Aladdin Investment Research API
  slug: investment-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-investment-research-openapi.yaml
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
