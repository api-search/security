---
api_specs:
- filename: peopledatalabs-autocomplete-api-openapi.yml
  format: yaml
  label: People Data Labs Autocomplete API
  slug: peopledatalabs-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-autocomplete-api-openapi.yml
- filename: peopledatalabs-cleaner-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Cleaner Endpoints API
  slug: peopledatalabs-cleaner-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-cleaner-endpoints-api-openapi.yml
- filename: peopledatalabs-company-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Company Endpoints API
  slug: peopledatalabs-company-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-company-endpoints-api-openapi.yml
- filename: peopledatalabs-ip-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs IP Enrichment API
  slug: peopledatalabs-ip-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-ip-enrichment-api-openapi.yml
- filename: peopledatalabs-job-title-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs Job Title Enrichment API
  slug: peopledatalabs-job-title-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-job-title-enrichment-api-openapi.yml
- filename: peopledatalabs-person-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Person Endpoints API
  slug: peopledatalabs-person-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-person-endpoints-api-openapi.yml
- filename: peopledatalabs-skill-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs Skill Enrichment API
  slug: peopledatalabs-skill-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-skill-enrichment-api-openapi.yml
- filename: peopledatalabs-subscription-api-openapi.yml
  format: yaml
  label: People Data Labs Subscription API
  slug: peopledatalabs-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-subscription-api-openapi.yml
- filename: peopledatalabs-preview-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs Preview Enrichment API
  slug: peopledatalabs-preview-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-preview-enrichment-api-openapi.yml
- filename: peopledatalabs-subject-request-api-openapi.yml
  format: yaml
  label: People Data Labs Subject Request API
  slug: peopledatalabs-subject-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-subject-request-api-openapi.yml
- filename: peopledatalabs-company-api-openapi.yml
  format: yaml
  label: People Data Labs Company API
  slug: peopledatalabs-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-company-api-openapi.yml
- filename: peopledatalabs-ip-api-openapi.yml
  format: yaml
  label: People Data Labs IP API
  slug: peopledatalabs-ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-ip-api-openapi.yml
- filename: peopledatalabs-jobs-api-openapi.yml
  format: yaml
  label: People Data Labs Jobs API
  slug: peopledatalabs-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-jobs-api-openapi.yml
- filename: peopledatalabs-person-api-openapi.yml
  format: yaml
  label: People Data Labs Person API
  slug: peopledatalabs-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-person-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: peopledatalabs.com
  spf: true
hosts:
- cert_expires: Oct 27 07:31:55 2026 GMT
  host: www.peopledatalabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 13:49:17 2026 GMT
  host: docs.peopledatalabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.peopledatalabs.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Peopledatalabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for People Data Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: People Data Labs
provider_slug: peopledatalabs
slug: peopledatalabs-domain-security
source_filename: peopledatalabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peopledatalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 07:31:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.peopledatalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:49:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.peopledatalabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: peopledatalabs.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/security/peopledatalabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Enrichment
- Web Intelligence
- Person Data
- Company Data
- B2B Data
- Contact Discovery
- Reference Data
- Firmographics
- Identity Resolution
---
