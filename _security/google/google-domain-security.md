---
api_specs:
- filename: books-api-openapi.yml
  format: yaml
  label: Books API
  slug: books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/books-api-openapi.yml
- filename: google-drive-api-openapi.yml
  format: yaml
  label: Google Drive API
  slug: google-drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-api-openapi.yml
- filename: google-drive-activity-api-openapi.yml
  format: yaml
  label: Google Drive Activity API
  slug: google-drive-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-activity-api-openapi.yml
- filename: google-drive-labels-api-openapi.yml
  format: yaml
  label: Google Drive Labels API
  slug: google-drive-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-labels-api-openapi.yml
- filename: google-calendar-api-openapi.yml
  format: yaml
  label: Google Calendar API
  slug: google-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-calendar-api-openapi.yml
- filename: google-gmail-api-openapi.yml
  format: yaml
  label: Google Gmail API
  slug: google-gmail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-gmail-api-openapi.yml
- filename: google-sheets-api-openapi.yml
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-sheets-api-openapi.yml
- filename: google-docs-api-openapi.yml
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-docs-api-openapi.yml
- filename: google-places-api-openapi.yml
  format: yaml
  label: Google Places API
  slug: google-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-places-api-openapi.yml
- filename: google-gemini-api-openapi.yml
  format: yaml
  label: Google Gemini API
  slug: google-gemini-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-gemini-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: workspace.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google
provider_slug: google
slug: google-domain-security
source_filename: google-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: workspace.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/security/google-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Cloud
- Developer
- Google
- Platform
- Search
- T1
---
