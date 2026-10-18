---
api_specs:
- filename: marketparquet-api-v1-api-openapi.yml
  format: yaml
  label: MarketParquet API V1 API
  slug: marketparquet-api-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketparquet/refs/heads/main/openapi/marketparquet-api-v1-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marketparquet.com
  spf: true
hosts:
- cert_expires: Dec  5 18:55:19 2026 GMT
  host: marketparquet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marketparquet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketParquet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MarketParquet
provider_slug: marketparquet
slug: marketparquet-domain-security
source_filename: marketparquet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketparquet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 18:55:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marketparquet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketparquet/refs/heads/main/security/marketparquet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Data
- MarketData
- APIs
---
