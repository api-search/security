---
api_specs:
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Events & Tracking API
  slug: leanplum-events-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum User & Device Attributes API
  slug: leanplum-user-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Messaging API
  slug: leanplum-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum A/B Tests API
  slug: leanplum-ab-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Content & Variables API
  slug: leanplum-content-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Data Export API
  slug: leanplum-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Postbacks & Batch API
  slug: leanplum-postbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leanplum.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.leanplum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:31:18 2026 GMT
  host: docs.leanplum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.leanplum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leanplum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leanplum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Leanplum
provider_slug: leanplum
slug: leanplum-domain-security
source_filename: leanplum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leanplum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n- host: docs.leanplum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:31:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.leanplum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: leanplum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/security/leanplum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile Marketing
- Customer Engagement
- Push Notifications
- Messaging
- A/B Testing
- Analytics
- CleverTap
---
