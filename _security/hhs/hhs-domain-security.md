---
api_specs:
- filename: hhs-agency-v1-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Agency v1 API
  slug: hhs-agency-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-agency-v1-api-openapi.yml
- filename: hhs-application-alpha-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Application Alpha API
  slug: hhs-application-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-application-alpha-api-openapi.yml
- filename: hhs-award-recommendation-alpha-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Award Recommendation Alpha API
  slug: hhs-award-recommendation-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-award-recommendation-alpha-api-openapi.yml
- filename: hhs-commongrants-protocol-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) CommonGrants Protocol API
  slug: hhs-commongrants-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-commongrants-protocol-api-openapi.yml
- filename: hhs-competition-alpha-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Competition Alpha API
  slug: hhs-competition-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-competition-alpha-api-openapi.yml
- filename: hhs-extract-v1-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Extract v1 API
  slug: hhs-extract-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-extract-v1-api-openapi.yml
- filename: hhs-file-v1-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) File v1 API
  slug: hhs-file-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-file-v1-api-openapi.yml
- filename: hhs-form-alpha-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Form Alpha API
  slug: hhs-form-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-form-alpha-api-openapi.yml
- filename: hhs-health-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Health API
  slug: hhs-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-health-api-openapi.yml
- filename: hhs-internal-v1-admin-only-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Internal v1 - Admin Only API
  slug: hhs-internal-v1-admin-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-internal-v1-admin-only-api-openapi.yml
- filename: hhs-local-only-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) LOCAL ONLY API
  slug: hhs-local-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-local-only-api-openapi.yml
- filename: hhs-opportunity-v1-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Opportunity v1 API
  slug: hhs-opportunity-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-opportunity-v1-api-openapi.yml
- filename: hhs-opportunity-v1-for-grantors-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Opportunity v1 - for Grantors API
  slug: hhs-opportunity-v1-for-grantors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-opportunity-v1-for-grantors-api-openapi.yml
- filename: hhs-organization-v1-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Organization v1 API
  slug: hhs-organization-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-organization-v1-api-openapi.yml
- filename: hhs-user-v1-internal-only-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) User v1 - Internal Only API
  slug: hhs-user-v1-internal-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-user-v1-internal-only-api-openapi.yml
- filename: hhs-workflow-api-openapi.yml
  format: yaml
  label: HHS (US Department of Health and Human Services) Workflow API
  slug: hhs-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/openapi/hhs-workflow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fda.gov
  spf: true
- caa:
  - 0 issue "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grants.gov
  spf: true
hosts:
- cert_expires: Oct  2 18:57:13 2026 GMT
  host: open.fda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 11:20:53 2026 GMT
  host: api.fda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 19:31:02 2026 GMT
  host: simpler.grants.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hhs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HHS (US Department of Health and Human Services), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HHS (US Department of Health and Human Services)
provider_slug: hhs
slug: hhs-domain-security
source_filename: hhs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:20:53 2026 GMT\n  hsts: null\n- host: simpler.grants.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 19:31:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fda.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: grants.gov\n  dnssec: false\n  caa:\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hhs/refs/heads/main/security/hhs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health
- Public Health
- Grants
- Interoperability
- FHIR
- Government
- Open Data
- FDA
- HRSA
- ONC
---
