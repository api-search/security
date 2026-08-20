---
api_specs:
- filename: cvat-annotations-api-openapi.yml
  format: yaml
  label: CVAT annotations API
  slug: cvat-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-annotations-api-openapi.yml
- filename: cvat-cloudstorages-api-openapi.yml
  format: yaml
  label: CVAT cloudstorages API
  slug: cvat-cloudstorages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-cloudstorages-api-openapi.yml
- filename: cvat-jobs-api-openapi.yml
  format: yaml
  label: CVAT jobs API
  slug: cvat-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-jobs-api-openapi.yml
- filename: cvat-labels-api-openapi.yml
  format: yaml
  label: CVAT labels API
  slug: cvat-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-labels-api-openapi.yml
- filename: cvat-memberships-api-openapi.yml
  format: yaml
  label: CVAT memberships API
  slug: cvat-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-memberships-api-openapi.yml
- filename: cvat-organizations-api-openapi.yml
  format: yaml
  label: CVAT organizations API
  slug: cvat-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-organizations-api-openapi.yml
- filename: cvat-projects-api-openapi.yml
  format: yaml
  label: CVAT projects API
  slug: cvat-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-projects-api-openapi.yml
- filename: cvat-tasks-api-openapi.yml
  format: yaml
  label: CVAT tasks API
  slug: cvat-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cvat.ai
  spf: true
hosts:
- cert_expires: Sep 29 13:46:05 2026 GMT
  host: www.cvat.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 08:50:04 2026 GMT
  host: app.cvat.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cvat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CVAT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CVAT
provider_slug: cvat
slug: cvat-domain-security
source_filename: cvat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cvat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:46:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.cvat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:50:04 2026 GMT\n  hsts: false\ndomains:\n- domain: cvat.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/security/cvat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Computer-Vision
- Data Annotation
- Labeling
- Datasets
- Open-Source
---
