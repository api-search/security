---
api_specs:
- filename: openswissdata-com-cantons-api-openapi.yml
  format: yaml
  label: Open Swiss Data Cantons API
  slug: openswissdata-com-cantons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openswissdata-com/openapi/openswissdata-com-cantons-api-openapi.yml
- filename: openswissdata-com-communes-api-openapi.yml
  format: yaml
  label: Open Swiss Data Communes API
  slug: openswissdata-com-communes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openswissdata-com/openapi/openswissdata-com-communes-api-openapi.yml
- filename: openswissdata-com-company-api-openapi.yml
  format: yaml
  label: Open Swiss Data Company API
  slug: openswissdata-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openswissdata-com/openapi/openswissdata-com-company-api-openapi.yml
- filename: openswissdata-com-datasets-api-openapi.yml
  format: yaml
  label: Open Swiss Data Datasets API
  slug: openswissdata-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openswissdata-com/openapi/openswissdata-com-datasets-api-openapi.yml
- filename: openswissdata-com-localities-api-openapi.yml
  format: yaml
  label: Open Swiss Data Localities API
  slug: openswissdata-com-localities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openswissdata-com/openapi/openswissdata-com-localities-api-openapi.yml
- filename: openswissdata-com-sources-api-openapi.yml
  format: yaml
  label: Open Swiss Data Sources API
  slug: openswissdata-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openswissdata-com/openapi/openswissdata-com-sources-api-openapi.yml
- filename: openswissdata-com-tariff-api-openapi.yml
  format: yaml
  label: Open Swiss Data Tariff API
  slug: openswissdata-com-tariff-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openswissdata-com/openapi/openswissdata-com-tariff-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: openswissdata.com
  spf: true
hosts:
- cert_expires: Dec 27 00:20:27 2026 GMT
  host: openswissdata.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Swiss Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Swiss Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Open Swiss Data
provider_slug: openswissdata-com
slug: openswissdata-com-domain-security
source_filename: openswissdata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openswissdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 00:20:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: openswissdata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/openswissdata-com/security/openswissdata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Finance
- Switzerland
- Open Data
---
