---
api_specs:
- filename: elastic-account-api-openapi.yml
  format: yaml
  label: Elastic Account API
  slug: elastic-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-account-api-openapi.yml
- filename: elastic-cluster-api-openapi.yml
  format: yaml
  label: Elastic Cluster API
  slug: elastic-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-cluster-api-openapi.yml
- filename: elastic-dataviews-api-openapi.yml
  format: yaml
  label: Elastic DataViews API
  slug: elastic-dataviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-dataviews-api-openapi.yml
- filename: elastic-deployments-api-openapi.yml
  format: yaml
  label: Elastic Deployments API
  slug: elastic-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-deployments-api-openapi.yml
- filename: elastic-documents-api-openapi.yml
  format: yaml
  label: Elastic Documents API
  slug: elastic-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-documents-api-openapi.yml
- filename: elastic-indices-api-openapi.yml
  format: yaml
  label: Elastic Indices API
  slug: elastic-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-indices-api-openapi.yml
- filename: elastic-savedobjects-api-openapi.yml
  format: yaml
  label: Elastic SavedObjects API
  slug: elastic-savedobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-savedobjects-api-openapi.yml
- filename: elastic-search-api-openapi.yml
  format: yaml
  label: Elastic Search API
  slug: elastic-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-search-api-openapi.yml
- filename: elastic-security-api-openapi.yml
  format: yaml
  label: Elastic Security API
  slug: elastic-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-security-api-openapi.yml
- filename: elastic-spaces-api-openapi.yml
  format: yaml
  label: Elastic Spaces API
  slug: elastic-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-spaces-api-openapi.yml
- filename: elastic-status-api-openapi.yml
  format: yaml
  label: Elastic Status API
  slug: elastic-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-status-api-openapi.yml
- filename: elastic-trafficfilters-api-openapi.yml
  format: yaml
  label: Elastic TrafficFilters API
  slug: elastic-trafficfilters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-trafficfilters-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elastic.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: elastic-cloud.com
  spf: true
hosts:
- cert_expires: Dec 12 21:06:03 2026 GMT
  host: www.elastic.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.elastic-cloud.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elastic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elastic, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elastic
provider_slug: elastic
slug: elastic-domain-security
source_filename: elastic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elastic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:06:03 2026 GMT\n  hsts: false\n- host: api.elastic-cloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: elastic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: elastic-cloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/security/elastic-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Search
- Analytics
- Observability
- Security
- Visualization
- Cloud
---
