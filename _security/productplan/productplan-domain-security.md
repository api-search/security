---
api_specs:
- filename: productplan-bars-api-openapi.yml
  format: yaml
  label: ProductPlan Bars API
  slug: productplan-bars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-bars-api-openapi.yml
- filename: productplan-discovery-api-openapi.yml
  format: yaml
  label: ProductPlan Discovery API
  slug: productplan-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-discovery-api-openapi.yml
- filename: productplan-launches-api-openapi.yml
  format: yaml
  label: ProductPlan Launches API
  slug: productplan-launches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-launches-api-openapi.yml
- filename: productplan-roadmaps-api-openapi.yml
  format: yaml
  label: ProductPlan Roadmaps API
  slug: productplan-roadmaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-roadmaps-api-openapi.yml
- filename: productplan-status-api-openapi.yml
  format: yaml
  label: ProductPlan Status API
  slug: productplan-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-status-api-openapi.yml
- filename: productplan-strategy-api-openapi.yml
  format: yaml
  label: ProductPlan Strategy API
  slug: productplan-strategy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-strategy-api-openapi.yml
- filename: productplan-teams-api-openapi.yml
  format: yaml
  label: ProductPlan Teams API
  slug: productplan-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-teams-api-openapi.yml
- filename: productplan-users-api-openapi.yml
  format: yaml
  label: ProductPlan Users API
  slug: productplan-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: productplan.com
  spf: true
hosts:
- cert_expires: Oct  5 23:29:14 2026 GMT
  host: www.productplan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 03:31:38 2026 GMT
  host: docs.productplan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: app.productplan.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Productplan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProductPlan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ProductPlan
provider_slug: productplan
slug: productplan-domain-security
source_filename: productplan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.productplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:29:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.productplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:31:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.productplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: productplan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/security/productplan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Road Mapping
- Product Management
- OKR
- Roadmaps
- Features
- Product Strategy
- Launches
- Discovery
- Integrations
---
