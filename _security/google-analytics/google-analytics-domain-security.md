---
api_specs:
- filename: google-analytics-accounts-api-openapi.yml
  format: yaml
  label: Google Analytics accounts API
  slug: google-analytics-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-accounts-api-openapi.yml
- filename: google-analytics-accountsummaries-api-openapi.yml
  format: yaml
  label: Google Analytics accountSummaries API
  slug: google-analytics-accountsummaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-accountsummaries-api-openapi.yml
- filename: google-analytics-data-api-openapi.yml
  format: yaml
  label: Google Analytics data API
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-data-api-openapi.yml
- filename: google-analytics-events-api-openapi.yml
  format: yaml
  label: Google Analytics Events API
  slug: google-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-events-api-openapi.yml
- filename: google-analytics-management-api-openapi.yml
  format: yaml
  label: Google Analytics management API
  slug: google-analytics-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-management-api-openapi.yml
- filename: google-analytics-metadata-api-openapi.yml
  format: yaml
  label: Google Analytics metadata API
  slug: google-analytics-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-metadata-api-openapi.yml
- filename: google-analytics-properties-api-openapi.yml
  format: yaml
  label: Google Analytics properties API
  slug: google-analytics-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-properties-api-openapi.yml
- filename: google-analytics-provisioning-api-openapi.yml
  format: yaml
  label: Google Analytics provisioning API
  slug: google-analytics-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-provisioning-api-openapi.yml
- filename: google-analytics-reports-api-openapi.yml
  format: yaml
  label: Google Analytics reports API
  slug: google-analytics-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-reports-api-openapi.yml
- filename: google-analytics-user-deletion-api-openapi.yml
  format: yaml
  label: Google Analytics User Deletion API
  slug: google-analytics-user-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-user-deletion-api-openapi.yml
- filename: google-analytics-useractivity-api-openapi.yml
  format: yaml
  label: Google Analytics userActivity API
  slug: google-analytics-useractivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-useractivity-api-openapi.yml
- filename: google-analytics-userdeletion-api-openapi.yml
  format: yaml
  label: Google Analytics userDeletion API
  slug: google-analytics-userdeletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-userdeletion-api-openapi.yml
- filename: google-analytics-validation-api-openapi.yml
  format: yaml
  label: Google Analytics Validation API
  slug: google-analytics-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-validation-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Oct 12 18:05:55 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:07:34 2026 GMT
  host: analyticsdata.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:07:34 2026 GMT
  host: analyticsadmin.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Analytics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Analytics
provider_slug: google-analytics
slug: google-analytics-domain-security
source_filename: google-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: analyticsdata.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:07:34 2026 GMT\n  hsts: null\n- host: analyticsadmin.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:07:34 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/security/google-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
---
