---
api_specs:
- filename: jane-app-appointments-api-openapi.yml
  format: yaml
  label: Jane Appointments API
  slug: jane-app-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-appointments-api-openapi.yml
- filename: jane-app-careplans-api-openapi.yml
  format: yaml
  label: Jane Care Plans API
  slug: jane-app-careplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-careplans-api-openapi.yml
- filename: jane-app-catalog-api-openapi.yml
  format: yaml
  label: Jane Catalog API
  slug: jane-app-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-catalog-api-openapi.yml
- filename: jane-app-company-api-openapi.yml
  format: yaml
  label: Jane Company API
  slug: jane-app-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-company-api-openapi.yml
- filename: jane-app-disciplines-api-openapi.yml
  format: yaml
  label: Jane Disciplines API
  slug: jane-app-disciplines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-disciplines-api-openapi.yml
- filename: jane-app-documentuploads-api-openapi.yml
  format: yaml
  label: Jane Document Uploads API
  slug: jane-app-documentuploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-documentuploads-api-openapi.yml
- filename: jane-app-extensions-api-openapi.yml
  format: yaml
  label: Jane Extensions API
  slug: jane-app-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-extensions-api-openapi.yml
- filename: jane-app-locations-api-openapi.yml
  format: yaml
  label: Jane Locations API
  slug: jane-app-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-locations-api-openapi.yml
- filename: jane-app-medications-api-openapi.yml
  format: yaml
  label: Jane Medications API
  slug: jane-app-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-medications-api-openapi.yml
- filename: jane-app-observations-api-openapi.yml
  format: yaml
  label: Jane Observations API
  slug: jane-app-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-observations-api-openapi.yml
- filename: jane-app-patients-api-openapi.yml
  format: yaml
  label: Jane Patients API
  slug: jane-app-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-patients-api-openapi.yml
- filename: jane-app-staffmembers-api-openapi.yml
  format: yaml
  label: Jane Staff Members API
  slug: jane-app-staffmembers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-staffmembers-api-openapi.yml
- filename: jane-app-treatments-api-openapi.yml
  format: yaml
  label: Jane Treatments API
  slug: jane-app-treatments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-treatments-api-openapi.yml
- filename: jane-app-webhooks-api-openapi.yml
  format: yaml
  label: Jane Webhooks API
  slug: jane-app-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jane.app
  spf: true
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jane.qa
  spf: false
hosts:
- cert_expires: Sep 11 19:57:27 2026 GMT
  host: jane.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 17:00:41 2026 GMT
  host: developers.jane.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: jdpdocsdemo.jane.qa
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jane App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jane, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jane
provider_slug: jane-app
slug: jane-app-domain-security
source_filename: jane-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jane.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:57:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.jane.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 17:00:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jdpdocsdemo.jane.qa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: jane.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: jane.qa\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/security/jane-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Canada
- Practice Management
- EHR
- EMR
- Scheduling
- Clinical Documentation
- Telehealth
- Health and Wellness
- REST API
- Authentication
- Webhook
---
