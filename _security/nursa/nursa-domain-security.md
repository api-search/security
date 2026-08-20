---
api_specs:
- filename: nursa-clinicians-api-openapi.yml
  format: yaml
  label: Nursa Clinicians API
  slug: nursa-clinicians-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-clinicians-api-openapi.yml
- filename: nursa-downloads-api-openapi.yml
  format: yaml
  label: Nursa Downloads API
  slug: nursa-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-downloads-api-openapi.yml
- filename: nursa-facilities-api-openapi.yml
  format: yaml
  label: Nursa Facilities API
  slug: nursa-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-facilities-api-openapi.yml
- filename: nursa-facilities-webhooks-api-openapi.yml
  format: yaml
  label: Nursa Facilities webhooks API
  slug: nursa-facilities-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-facilities-webhooks-api-openapi.yml
- filename: nursa-licenses-api-openapi.yml
  format: yaml
  label: Nursa Licenses API
  slug: nursa-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-licenses-api-openapi.yml
- filename: nursa-marketplace-api-openapi.yml
  format: yaml
  label: Nursa Marketplace API
  slug: nursa-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-marketplace-api-openapi.yml
- filename: nursa-scheduled-shifts-api-openapi.yml
  format: yaml
  label: Nursa Scheduled shifts API
  slug: nursa-scheduled-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-scheduled-shifts-api-openapi.yml
- filename: nursa-shift-reports-api-openapi.yml
  format: yaml
  label: Nursa Shift reports API
  slug: nursa-shift-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shift-reports-api-openapi.yml
- filename: nursa-shift-requests-api-openapi.yml
  format: yaml
  label: Nursa Shift requests API
  slug: nursa-shift-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shift-requests-api-openapi.yml
- filename: nursa-shifts-api-openapi.yml
  format: yaml
  label: Nursa Shifts API
  slug: nursa-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shifts-api-openapi.yml
- filename: nursa-support-api-openapi.yml
  format: yaml
  label: Nursa Support API
  slug: nursa-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-support-api-openapi.yml
- filename: nursa-user-webhooks-api-openapi.yml
  format: yaml
  label: Nursa User webhooks API
  slug: nursa-user-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-user-webhooks-api-openapi.yml
- filename: nursa-webhook-logs-api-openapi.yml
  format: yaml
  label: Nursa Webhook logs API
  slug: nursa-webhook-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-webhook-logs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nursa.com
  spf: true
hosts:
- cert_expires: Oct 17 19:30:52 2026 GMT
  host: nursa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 19:52:52 2026 GMT
  host: developers.prod.nursa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 22:56:19 2026 GMT
  host: docs.nursa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nursa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nursa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nursa
provider_slug: nursa
slug: nursa-domain-security
source_filename: nursa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nursa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 19:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.prod.nursa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 19:52:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nursa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:56:19 2026 GMT\n  hsts: false\ndomains:\n- domain: nursa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/security/nursa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health
- Staffing
- Nursing
- Marketplace
- Workforce Management
- Scheduling
- Human Resources
- Per Diem
- Shifts
- Webhook
---
