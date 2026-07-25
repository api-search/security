---
api_specs:
- filename: cycloid-cloudcost-api-openapi.yml
  format: yaml
  label: Cycloid CloudCost API
  slug: cycloid-cloudcost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-cloudcost-api-openapi.yml
- filename: cycloid-configrepositories-api-openapi.yml
  format: yaml
  label: Cycloid ConfigRepositories API
  slug: cycloid-configrepositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-configrepositories-api-openapi.yml
- filename: cycloid-credentials-api-openapi.yml
  format: yaml
  label: Cycloid Credentials API
  slug: cycloid-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-credentials-api-openapi.yml
- filename: cycloid-inventory-api-openapi.yml
  format: yaml
  label: Cycloid Inventory API
  slug: cycloid-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-inventory-api-openapi.yml
- filename: cycloid-organizations-api-openapi.yml
  format: yaml
  label: Cycloid Organizations API
  slug: cycloid-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-organizations-api-openapi.yml
- filename: cycloid-pipelines-api-openapi.yml
  format: yaml
  label: Cycloid Pipelines API
  slug: cycloid-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-pipelines-api-openapi.yml
- filename: cycloid-projects-api-openapi.yml
  format: yaml
  label: Cycloid Projects API
  slug: cycloid-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-projects-api-openapi.yml
- filename: cycloid-servicecatalogs-api-openapi.yml
  format: yaml
  label: Cycloid ServiceCatalogs API
  slug: cycloid-servicecatalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-servicecatalogs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cycloid.io
  spf: true
hosts:
- cert_expires: Oct  9 02:02:42 2026 GMT
  host: www.cycloid.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 18:07:33 2026 GMT
  host: docs.cycloid.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 18:07:33 2026 GMT
  host: http-api.cycloid.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cycloid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cycloid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cycloid
provider_slug: cycloid
slug: cycloid-domain-security
source_filename: cycloid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cycloid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:02:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cycloid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:07:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: http-api.cycloid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:07:33 2026 GMT\n  hsts: null\ndomains:\n- domain: cycloid.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/security/cycloid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asset Inventory
- CI/CD
- Cloud Cost Management
- Cloud Management
- Developer Experience
- DevOps
- FinOps
- GitOps
- GreenOps
- Infrastructure as Code
- Internal Developer Platform
- Internal Developer Portal
- Multi-Cloud
- Platform Engineering
- RBAC
- Self-Service
- Service Catalog
- StackForms
- Terraform
---
