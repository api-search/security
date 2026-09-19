---
api_specs:
- filename: cloudchipr-accounts-api-openapi.yml
  format: yaml
  label: CloudChipr Accounts API
  slug: cloudchipr-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-accounts-api-openapi.yml
- filename: cloudchipr-budgets-api-openapi.yml
  format: yaml
  label: CloudChipr Budgets API
  slug: cloudchipr-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-budgets-api-openapi.yml
- filename: cloudchipr-categories-api-openapi.yml
  format: yaml
  label: CloudChipr Categories API
  slug: cloudchipr-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-categories-api-openapi.yml
- filename: cloudchipr-custom-data-api-openapi.yml
  format: yaml
  label: CloudChipr Custom Data API
  slug: cloudchipr-custom-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-custom-data-api-openapi.yml
- filename: cloudchipr-dashboards-api-openapi.yml
  format: yaml
  label: CloudChipr Dashboards API
  slug: cloudchipr-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-dashboards-api-openapi.yml
- filename: cloudchipr-filters-api-openapi.yml
  format: yaml
  label: CloudChipr Filters API
  slug: cloudchipr-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-filters-api-openapi.yml
- filename: cloudchipr-regions-api-openapi.yml
  format: yaml
  label: CloudChipr Regions API
  slug: cloudchipr-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-regions-api-openapi.yml
- filename: cloudchipr-resource-explorer-api-openapi.yml
  format: yaml
  label: CloudChipr Resource Explorer API
  slug: cloudchipr-resource-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-resource-explorer-api-openapi.yml
- filename: cloudchipr-resources-api-openapi.yml
  format: yaml
  label: CloudChipr Resources API
  slug: cloudchipr-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-resources-api-openapi.yml
- filename: cloudchipr-savings-opportunities-api-openapi.yml
  format: yaml
  label: CloudChipr Savings Opportunities API
  slug: cloudchipr-savings-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-savings-opportunities-api-openapi.yml
- filename: cloudchipr-widgets-api-openapi.yml
  format: yaml
  label: CloudChipr Widgets API
  slug: cloudchipr-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-widgets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloudchipr.com
  spf: true
hosts:
- cert_expires: Oct 14 15:37:05 2026 GMT
  host: cloudchipr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 03:08:58 2026 GMT
  host: api.cloudchipr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 21:34:42 2026 GMT
  host: docs.cloudchipr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cloudchipr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudChipr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CloudChipr
provider_slug: cloudchipr
slug: cloudchipr-domain-security
source_filename: cloudchipr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudchipr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:37:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cloudchipr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 03:08:58 2026 GMT\n  hsts: null\n- host: docs.cloudchipr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 21:34:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudchipr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/security/cloudchipr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Azure
- Cloud Cost Management
- Cost Optimization
- FinOps
- GCP
- Multi-Cloud
- Resource Cleanup
- Rightsizing
---
