---
api_specs:
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze People API
  slug: breeze-chms-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Tags API
  slug: breeze-chms-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Events API
  slug: breeze-chms-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Check-Ins and Attendance API
  slug: breeze-chms-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Giving and Contributions API
  slug: breeze-chms-giving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Funds API
  slug: breeze-chms-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Pledges API
  slug: breeze-chms-pledges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Forms API
  slug: breeze-chms-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Volunteers API
  slug: breeze-chms-volunteers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Account API
  slug: breeze-chms-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: breezechms.com
  spf: true
hosts:
- cert_expires: Sep 30 11:43:44 2026 GMT
  host: www.breezechms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: app.breezechms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Breeze Chms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breeze ChMS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Breeze ChMS
provider_slug: breeze-chms
slug: breeze-chms-domain-security
source_filename: breeze-chms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breezechms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:43:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.breezechms.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: breezechms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/security/breeze-chms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Church Management
- ChMS
- Nonprofit
- Giving
- Membership
- Events
- Faith
---
