---
api_specs:
- filename: seven-bridges-action-api-openapi.yml
  format: yaml
  label: Seven Bridges Action API
  slug: seven-bridges-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-action-api-openapi.yml
- filename: seven-bridges-api-settings-api-openapi.yml
  format: yaml
  label: Seven Bridges API Settings API
  slug: seven-bridges-api-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-api-settings-api-openapi.yml
- filename: seven-bridges-apps-api-openapi.yml
  format: yaml
  label: Seven Bridges Apps API
  slug: seven-bridges-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-apps-api-openapi.yml
- filename: seven-bridges-billing-api-openapi.yml
  format: yaml
  label: Seven Bridges Billing API
  slug: seven-bridges-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-billing-api-openapi.yml
- filename: seven-bridges-bulk-api-openapi.yml
  format: yaml
  label: Seven Bridges Bulk API
  slug: seven-bridges-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-bulk-api-openapi.yml
- filename: seven-bridges-files-api-openapi.yml
  format: yaml
  label: Seven Bridges Files API
  slug: seven-bridges-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-files-api-openapi.yml
- filename: seven-bridges-https-api-openapi.yml
  format: yaml
  label: 'Seven Bridges Https: API'
  slug: seven-bridges-https-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-https-api-openapi.yml
- filename: seven-bridges-projects-api-openapi.yml
  format: yaml
  label: Seven Bridges Projects API
  slug: seven-bridges-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-projects-api-openapi.yml
- filename: seven-bridges-rate-limit-api-openapi.yml
  format: yaml
  label: Seven Bridges Rate Limit API
  slug: seven-bridges-rate-limit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-rate-limit-api-openapi.yml
- filename: seven-bridges-search-api-openapi.yml
  format: yaml
  label: Seven Bridges Search API
  slug: seven-bridges-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-search-api-openapi.yml
- filename: seven-bridges-seven-bridges-platform-api-openapi.yml
  format: yaml
  label: Seven Bridges Seven Bridges Platform API
  slug: seven-bridges-seven-bridges-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-seven-bridges-platform-api-openapi.yml
- filename: seven-bridges-storage-api-openapi.yml
  format: yaml
  label: Seven Bridges Storage API
  slug: seven-bridges-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-storage-api-openapi.yml
- filename: seven-bridges-tasks-api-openapi.yml
  format: yaml
  label: Seven Bridges Tasks API
  slug: seven-bridges-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-tasks-api-openapi.yml
- filename: seven-bridges-upload-api-openapi.yml
  format: yaml
  label: Seven Bridges Upload API
  slug: seven-bridges-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-upload-api-openapi.yml
- filename: seven-bridges-user-api-openapi.yml
  format: yaml
  label: Seven Bridges User API
  slug: seven-bridges-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-user-api-openapi.yml
- filename: seven-bridges-users-api-openapi.yml
  format: yaml
  label: Seven Bridges Users API
  slug: seven-bridges-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sevenbridges.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sbgenomics.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.sevenbridges.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:03:30 2026 GMT
  host: docs.sevenbridges.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.sbgenomics.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Seven Bridges Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seven Bridges, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Seven Bridges
provider_slug: seven-bridges
slug: seven-bridges-domain-security
source_filename: seven-bridges-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sevenbridges.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: docs.sevenbridges.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:03:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sbgenomics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sevenbridges.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sbgenomics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/security/seven-bridges-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Genomics
- Bioinformatics
- Life Sciences
- Healthcare
- Cloud Computing
- Data Analysis
- Workflow-Automation
- Research
- Precision Medicine
- Common Workflow Language
- File Storage
- Company
---
