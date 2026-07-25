---
api_specs:
- filename: parseflow-admin-api-openapi.yml
  format: yaml
  label: Parseflow Admin API
  slug: parseflow-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-admin-api-openapi.yml
- filename: parseflow-analyze-api-openapi.yml
  format: yaml
  label: Parseflow Analyze API
  slug: parseflow-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-analyze-api-openapi.yml
- filename: parseflow-batch-api-openapi.yml
  format: yaml
  label: Parseflow Batch API
  slug: parseflow-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-batch-api-openapi.yml
- filename: parseflow-billing-api-openapi.yml
  format: yaml
  label: Parseflow Billing API
  slug: parseflow-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-billing-api-openapi.yml
- filename: parseflow-health-api-openapi.yml
  format: yaml
  label: Parseflow Health API
  slug: parseflow-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-health-api-openapi.yml
- filename: parseflow-index-api-openapi.yml
  format: yaml
  label: Parseflow Index API
  slug: parseflow-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-index-api-openapi.yml
- filename: parseflow-jobs-api-openapi.yml
  format: yaml
  label: Parseflow Jobs API
  slug: parseflow-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-jobs-api-openapi.yml
- filename: parseflow-me-api-openapi.yml
  format: yaml
  label: Parseflow Me API
  slug: parseflow-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-me-api-openapi.yml
- filename: parseflow-pack-api-openapi.yml
  format: yaml
  label: Parseflow Pack API
  slug: parseflow-pack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-pack-api-openapi.yml
- filename: parseflow-process-api-openapi.yml
  format: yaml
  label: Parseflow Process API
  slug: parseflow-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-process-api-openapi.yml
- filename: parseflow-search-api-openapi.yml
  format: yaml
  label: Parseflow Search API
  slug: parseflow-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-search-api-openapi.yml
- filename: parseflow-stats-api-openapi.yml
  format: yaml
  label: Parseflow Stats API
  slug: parseflow-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-stats-api-openapi.yml
- filename: parseflow-usage-api-openapi.yml
  format: yaml
  label: Parseflow Usage API
  slug: parseflow-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-usage-api-openapi.yml
- filename: parseflow-webhooks-api-openapi.yml
  format: yaml
  label: Parseflow Webhooks API
  slug: parseflow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parseflow.tech
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azurecontainerapps.io
  spf: false
hosts:
- cert_expires: Oct  2 03:54:26 2026 GMT
  host: docs.parseflow.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: parseflow-api.thankfulisland-fec0f8f2.westus2.azurecontainerapps.io
  https: false
kind: domain-security
layout: security
method: probed
name: Parseflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parseflow, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Parseflow
provider_slug: parseflow
slug: parseflow-domain-security
source_filename: parseflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.parseflow.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:54:26 2026 GMT\n  hsts: false\n- host: parseflow-api.thankfulisland-fec0f8f2.westus2.azurecontainerapps.io\n  https: false\ndomains:\n- domain: parseflow.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: azurecontainerapps.io\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/security/parseflow-domain-security.yml
summary_line: TLSv1.3
tags:
- Document Parsing
- PDF
- OCR
- Text Extraction
- Document AI
- Search
- BYOK
- Async Jobs
- Webhooks
- REST
---
