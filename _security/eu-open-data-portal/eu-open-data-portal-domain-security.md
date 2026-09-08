---
api_specs:
- filename: eu-open-data-portal-hub-search-openapi.yaml
  format: yaml
  label: EU Open Data Portal Search API (hub-search)
  slug: eu-open-data-portal-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-hub-search-openapi.yaml
- filename: eu-open-data-portal-hub-repo-openapi.yaml
  format: yaml
  label: EU Open Data Portal Registry API (hub-repo)
  slug: eu-open-data-portal-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-hub-repo-openapi.yaml
- filename: eu-open-data-portal-mqa-metrics-cache-openapi.yaml
  format: yaml
  label: EU Open Data Portal MQA Metrics Cache API
  slug: eu-open-data-portal-mqa-metrics-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-mqa-metrics-cache-openapi.yaml
- filename: eu-open-data-portal-mqa-shacl-openapi.yaml
  format: yaml
  label: EU Open Data Portal SHACL Validation API
  slug: eu-open-data-portal-mqa-shacl-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-mqa-shacl-openapi.yaml
- filename: eu-open-data-portal-mqa-reporter-openapi.yaml
  format: yaml
  label: EU Open Data Portal MQA Metrics Reporter API
  slug: eu-open-data-portal-mqa-metrics-reporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-mqa-reporter-openapi.yaml
- filename: eu-open-data-portal-hub-statistics-swagger.json
  format: json
  label: EU Open Data Portal Statistics API
  slug: eu-open-data-portal-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-hub-statistics-swagger.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: europa.eu
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: data.europa.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eu Open Data Portal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EU Open Data Portal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: EU Open Data Portal
provider_slug: eu-open-data-portal
slug: eu-open-data-portal-domain-security
source_filename: eu-open-data-portal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.europa.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: europa.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/security/eu-open-data-portal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Government
- Open Data
- SPARQL
- EU
- Regulatory
- Linked Data
- DCAT-AP
- Data Quality
- Metadata
- Catalogs
---
