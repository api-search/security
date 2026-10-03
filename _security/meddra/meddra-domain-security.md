---
api_specs:
- filename: meddra-dataimpact-api-openapi.yml
  format: yaml
  label: Meddra Data Impact API
  slug: meddra-dataimpact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-dataimpact-api-openapi.yml
- filename: meddra-details-api-openapi.yml
  format: yaml
  label: Meddra Details API
  slug: meddra-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-details-api-openapi.yml
- filename: meddra-download-api-openapi.yml
  format: yaml
  label: Meddra Download API
  slug: meddra-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-download-api-openapi.yml
- filename: meddra-export-api-openapi.yml
  format: yaml
  label: Meddra Export API
  slug: meddra-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-export-api-openapi.yml
- filename: meddra-gettop-api-openapi.yml
  format: yaml
  label: Meddra Get Top API
  slug: meddra-gettop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-gettop-api-openapi.yml
- filename: meddra-hierarchy-api-openapi.yml
  format: yaml
  label: Meddra Hierarchy API
  slug: meddra-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-hierarchy-api-openapi.yml
- filename: meddra-history-api-openapi.yml
  format: yaml
  label: Meddra History API
  slug: meddra-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-history-api-openapi.yml
- filename: meddra-language-api-openapi.yml
  format: yaml
  label: Meddra Language API
  slug: meddra-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-language-api-openapi.yml
- filename: meddra-release-api-openapi.yml
  format: yaml
  label: Meddra Release API
  slug: meddra-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-release-api-openapi.yml
- filename: meddra-search-api-openapi.yml
  format: yaml
  label: Meddra Search API
  slug: meddra-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-search-api-openapi.yml
- filename: meddra-smq-api-openapi.yml
  format: yaml
  label: Meddra SMQ API
  slug: meddra-smq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-smq-api-openapi.yml
- filename: meddra-status-api-openapi.yml
  format: yaml
  label: Meddra Status API
  slug: meddra-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-status-api-openapi.yml
- filename: meddra-svalidation-api-openapi.yml
  format: yaml
  label: Meddra S Validation API
  slug: meddra-svalidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-svalidation-api-openapi.yml
- filename: meddra-type-api-openapi.yml
  format: yaml
  label: Meddra Type API
  slug: meddra-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-type-api-openapi.yml
- filename: meddra-versionr-api-openapi.yml
  format: yaml
  label: Meddra Version R API
  slug: meddra-versionr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-versionr-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: meddra.org
  spf: true
hosts:
- cert_expires: Nov 22 14:04:49 2026 GMT
  host: www.meddra.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 14:04:49 2026 GMT
  host: mapisbx.meddra.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Meddra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meddra, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Meddra
provider_slug: meddra
slug: meddra-domain-security
source_filename: meddra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meddra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 14:04:49 2026 GMT\n  hsts: false\n- host: mapisbx.meddra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 14:04:49 2026 GMT\n  hsts: null\ndomains:\n- domain: meddra.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/security/meddra-domain-security.yml
summary_line: TLSv1.3
tags:
- Medical Terminology
- Pharmacovigilance
- Drug Safety
- Adverse Events
- Regulatory
- Clinical Trials
- Healthcare
- Life Sciences
- Standards
- Ontology
---
