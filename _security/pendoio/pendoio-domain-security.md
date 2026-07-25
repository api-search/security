---
api_specs:
- filename: pendoio-account-api-openapi.yml
  format: yaml
  label: Pendo.io Account API
  slug: pendoio-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-account-api-openapi.yml
- filename: pendoio-admin-api-openapi.yml
  format: yaml
  label: Pendo.io Admin API
  slug: pendoio-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-admin-api-openapi.yml
- filename: pendoio-aggregation-api-openapi.yml
  format: yaml
  label: Pendo.io Aggregation API
  slug: pendoio-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-aggregation-api-openapi.yml
- filename: pendoio-bulk-deletion-gdpr-ccpa-api-openapi.yml
  format: yaml
  label: Pendo.io Bulk Deletion (GDPR/CCPA) API
  slug: pendoio-bulk-deletion-gdpr-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-bulk-deletion-gdpr-ccpa-api-openapi.yml
- filename: pendoio-conversations-api-openapi.yml
  format: yaml
  label: Pendo.io Conversations API
  slug: pendoio-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-conversations-api-openapi.yml
- filename: pendoio-data-sync-api-openapi.yml
  format: yaml
  label: Pendo.io Data Sync API
  slug: pendoio-data-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-data-sync-api-openapi.yml
- filename: pendoio-exclude-lists-servers-api-openapi.yml
  format: yaml
  label: Pendo.io Exclude Lists & Servers API
  slug: pendoio-exclude-lists-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-exclude-lists-servers-api-openapi.yml
- filename: pendoio-feature-api-openapi.yml
  format: yaml
  label: Pendo.io Feature API
  slug: pendoio-feature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-feature-api-openapi.yml
- filename: pendoio-guide-api-openapi.yml
  format: yaml
  label: Pendo.io Guide API
  slug: pendoio-guide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-guide-api-openapi.yml
- filename: pendoio-listen-api-openapi.yml
  format: yaml
  label: Pendo.io Listen API
  slug: pendoio-listen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-listen-api-openapi.yml
- filename: pendoio-metadata-api-openapi.yml
  format: yaml
  label: Pendo.io Metadata API
  slug: pendoio-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-metadata-api-openapi.yml
- filename: pendoio-page-api-openapi.yml
  format: yaml
  label: Pendo.io Page API
  slug: pendoio-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-page-api-openapi.yml
- filename: pendoio-report-api-openapi.yml
  format: yaml
  label: Pendo.io Report API
  slug: pendoio-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-report-api-openapi.yml
- filename: pendoio-segment-api-openapi.yml
  format: yaml
  label: Pendo.io Segment API
  slug: pendoio-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-segment-api-openapi.yml
- filename: pendoio-track-api-openapi.yml
  format: yaml
  label: Pendo.io Track API
  slug: pendoio-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-track-api-openapi.yml
- filename: pendoio-visitor-api-openapi.yml
  format: yaml
  label: Pendo.io Visitor API
  slug: pendoio-visitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-visitor-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pendo.io
  spf: true
hosts:
- cert_expires: Oct 17 04:14:07 2026 GMT
  host: app.pendo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 03:58:57 2026 GMT
  host: us1.app.pendo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 07:17:23 2026 GMT
  host: app.eu.pendo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pendoio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pendo.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pendo.io
provider_slug: pendoio
slug: pendoio-domain-security
source_filename: pendoio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 04:14:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us1.app.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:58:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.eu.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:17:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pendo.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/security/pendoio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Product Analytics
- Product Experience
- Digital Adoption
- User Analytics
- In-App Guidance
- Customer Feedback
- SaaS
---
