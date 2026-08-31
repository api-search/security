---
api_specs:
- filename: metabolon-assistant-api-openapi.yml
  format: yaml
  label: Metabolon Assistant API
  slug: metabolon-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-assistant-api-openapi.yml
- filename: metabolon-auth-api-openapi.yml
  format: yaml
  label: Metabolon Auth API
  slug: metabolon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-auth-api-openapi.yml
- filename: metabolon-decentralization-api-openapi.yml
  format: yaml
  label: Metabolon Decentralization API
  slug: metabolon-decentralization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-decentralization-api-openapi.yml
- filename: metabolon-eula-api-openapi.yml
  format: yaml
  label: Metabolon Eula API
  slug: metabolon-eula-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-eula-api-openapi.yml
- filename: metabolon-files-api-openapi.yml
  format: yaml
  label: Metabolon Files API
  slug: metabolon-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-files-api-openapi.yml
- filename: metabolon-health-api-openapi.yml
  format: yaml
  label: Metabolon Health API
  slug: metabolon-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-health-api-openapi.yml
- filename: metabolon-labvantagefiles-api-openapi.yml
  format: yaml
  label: Metabolon Lab Vantage Files API
  slug: metabolon-labvantagefiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-labvantagefiles-api-openapi.yml
- filename: metabolon-pipelinestatus-api-openapi.yml
  format: yaml
  label: Metabolon Pipeline Status API
  slug: metabolon-pipelinestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-pipelinestatus-api-openapi.yml
- filename: metabolon-projects-api-openapi.yml
  format: yaml
  label: Metabolon Projects API
  slug: metabolon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-projects-api-openapi.yml
- filename: metabolon-reports-api-openapi.yml
  format: yaml
  label: Metabolon Reports API
  slug: metabolon-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-reports-api-openapi.yml
- filename: metabolon-samplesets-api-openapi.yml
  format: yaml
  label: Metabolon Sample Sets API
  slug: metabolon-samplesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-samplesets-api-openapi.yml
- filename: metabolon-samplesetsinfo-api-openapi.yml
  format: yaml
  label: Metabolon Sample Sets Info API
  slug: metabolon-samplesetsinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-samplesetsinfo-api-openapi.yml
- filename: metabolon-search-api-openapi.yml
  format: yaml
  label: Metabolon Search API
  slug: metabolon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-search-api-openapi.yml
- filename: metabolon-sharedfile-api-openapi.yml
  format: yaml
  label: Metabolon Shared File API
  slug: metabolon-sharedfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-sharedfile-api-openapi.yml
- filename: metabolon-spectraldata-api-openapi.yml
  format: yaml
  label: Metabolon Spectral Data API
  slug: metabolon-spectraldata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-spectraldata-api-openapi.yml
- filename: metabolon-status-api-openapi.yml
  format: yaml
  label: Metabolon Status API
  slug: metabolon-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-status-api-openapi.yml
- filename: metabolon-studybuilder-api-openapi.yml
  format: yaml
  label: Metabolon Study Builder API
  slug: metabolon-studybuilder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-studybuilder-api-openapi.yml
- filename: metabolon-users-api-openapi.yml
  format: yaml
  label: Metabolon Users API
  slug: metabolon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metabolon.com
  spf: false
hosts:
- cert_expires: Oct 28 02:32:01 2026 GMT
  host: www.metabolon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: portal-api.prod.metabolon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: discovery.prod.metabolon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metabolon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metabolon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Metabolon
provider_slug: metabolon
slug: metabolon-domain-security
source_filename: metabolon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metabolon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 02:32:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal-api.prod.metabolon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\n- host: discovery.prod.metabolon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: metabolon.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/security/metabolon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Metabolomics
- Life Sciences
- Bioinformatics
- Multiomics
- Biotechnology
- Drug Discovery
- Precision Medicine
- Microbiome
- Biomarkers
- Contract Research
- Laboratory
---
