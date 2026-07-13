---
api_specs:
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Candidates API
  slug: checkr-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Invitations API
  slug: checkr-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Reports API
  slug: checkr-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Screenings API
  slug: checkr-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Verifications API
  slug: checkr-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Packages API
  slug: checkr-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Documents API
  slug: checkr-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Adverse Actions API
  slug: checkr-adverse-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Subscriptions API
  slug: checkr-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Continuous Checks API
  slug: checkr-continuous-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Nodes and Hierarchy API
  slug: checkr-nodes-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Geos API
  slug: checkr-geos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Webhooks API
  slug: checkr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: checkr.com
  spf: true
hosts:
- cert_expires: Aug 16 21:14:21 2026 GMT
  host: checkr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 07:19:28 2026 GMT
  host: docs.checkr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 21:19:13 2026 GMT
  host: api.checkr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Checkr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Checkr
provider_slug: checkr
slug: checkr-domain-security
source_filename: checkr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: checkr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 21:14:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.checkr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:19:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.checkr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:19:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: checkr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/security/checkr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Background Checks
- Employment Screening
- Compliance
- HR Tech
- Identity Verification
- Criminal Records
---
