---
api_specs:
- filename: affinda-documents-api-openapi.yml
  format: yaml
  label: Affinda Documents API
  slug: affinda-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-documents-api-openapi.yml
- filename: affinda-document-types-api-openapi.yml
  format: yaml
  label: Affinda Document Types API
  slug: affinda-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-document-types-api-openapi.yml
- filename: affinda-extractors-api-openapi.yml
  format: yaml
  label: Affinda Extractors API
  slug: affinda-extractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-extractors-api-openapi.yml
- filename: affinda-document-splitters-api-openapi.yml
  format: yaml
  label: Affinda Document Splitters API
  slug: affinda-document-splitters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-document-splitters-api-openapi.yml
- filename: affinda-workspaces-api-openapi.yml
  format: yaml
  label: Affinda Workspaces API
  slug: affinda-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-workspaces-api-openapi.yml
- filename: affinda-organizations-api-openapi.yml
  format: yaml
  label: Affinda Organizations API
  slug: affinda-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-organizations-api-openapi.yml
- filename: affinda-invitations-api-openapi.yml
  format: yaml
  label: Affinda Invitations API
  slug: affinda-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-invitations-api-openapi.yml
- filename: affinda-data-sources-api-openapi.yml
  format: yaml
  label: Affinda Data Sources API
  slug: affinda-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-data-sources-api-openapi.yml
- filename: affinda-annotations-api-openapi.yml
  format: yaml
  label: Affinda Annotations API
  slug: affinda-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-annotations-api-openapi.yml
- filename: affinda-validation-results-api-openapi.yml
  format: yaml
  label: Affinda Validation Results API
  slug: affinda-validation-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-validation-results-api-openapi.yml
- filename: affinda-tags-api-openapi.yml
  format: yaml
  label: Affinda Tags API
  slug: affinda-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-tags-api-openapi.yml
- filename: affinda-usage-api-openapi.yml
  format: yaml
  label: Affinda Usage API
  slug: affinda-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-usage-api-openapi.yml
- filename: affinda-webhooks-api-openapi.yml
  format: yaml
  label: Affinda Webhooks API
  slug: affinda-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-webhooks-api-openapi.yml
- filename: affinda-search-match-api-openapi.yml
  format: yaml
  label: Affinda Search and Match API
  slug: affinda-search-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-search-match-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:netops@draftable.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: affinda.com
  spf: true
hosts:
- cert_expires: Oct  5 16:55:24 2026 GMT
  host: www.affinda.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:47:43 2026 GMT
  host: docs.affinda.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Affinda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affinda, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Affinda
provider_slug: affinda
slug: affinda-domain-security
source_filename: affinda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.affinda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:55:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.affinda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:47:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: affinda.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:netops@draftable.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/security/affinda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Document Processing
- Intelligent Document Processing
- IDP
- OCR
- Resume Parsing
- Invoice Parsing
- Receipt Parsing
- Document Extraction
- Document Classification
- Document Splitting
- Recruitment
- Banking
- Insurance
- Logistics
- Healthcare
- Government
---
