---
api_specs:
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Registry API
  slug: benchling-lims-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Sequences API
  slug: benchling-lims-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Inventory API
  slug: benchling-lims-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Notebook (Entries) API
  slug: benchling-lims-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Assay Results & Runs API
  slug: benchling-lims-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Workflows API
  slug: benchling-lims-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Requests API
  slug: benchling-lims-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Events API
  slug: benchling-lims-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Apps & Webhooks API
  slug: benchling-lims-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Organizations & Users API
  slug: benchling-lims-org-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
- filename: benchling-lims-openapi.yml
  format: yaml
  label: Benchling Blobs & Files API
  slug: benchling-lims-blobs-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/openapi/benchling-lims-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: benchling.com
  spf: true
hosts:
- cert_expires: Aug 19 07:31:55 2026 GMT
  host: www.benchling.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:58:36 2026 GMT
  host: docs.benchling.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Benchling Lims Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benchling, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Benchling
provider_slug: benchling-lims
slug: benchling-lims-domain-security
source_filename: benchling-lims-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benchling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:31:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.benchling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:58:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: benchling.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/security/benchling-lims-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Life Sciences
- Biotech
- LIMS
- Electronic Lab Notebook
- Registry
- Molecular Biology
- Inventory Management
- Assay Management
- Workflows
- Webhooks
- REST
---
