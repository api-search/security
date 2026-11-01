---
api_specs:
- filename: quantsonar-com-default-api-openapi.yml
  format: yaml
  label: quantsonar-com 分红送股 API
  slug: quantsonar-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quantsonar-com/openapi/quantsonar-com-default-api-openapi.yml
- filename: quantsonar-com-etf-api-openapi.yml
  format: yaml
  label: quantsonar-com ETF API
  slug: quantsonar-com-etf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quantsonar-com/openapi/quantsonar-com-etf-api-openapi.yml
- filename: quantsonar-com-health-api-openapi.yml
  format: yaml
  label: quantsonar-com Health API
  slug: quantsonar-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quantsonar-com/openapi/quantsonar-com-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quantsonar.com
  spf: true
hosts:
- cert_expires: Dec 12 18:06:24 2026 GMT
  host: quantsonar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quantsonar Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for quantsonar-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: quantsonar-com
provider_slug: quantsonar-com
slug: quantsonar-com-domain-security
source_filename: quantsonar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quantsonar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 18:06:24 2026 GMT\n  hsts: null\ndomains:\n- domain: quantsonar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/quantsonar-com/security/quantsonar-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Finance
- Data
- API
- China
- Stock-Market
---
