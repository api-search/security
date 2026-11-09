---
api_specs:
- filename: google-drive-files-api-openapi.yml
  format: yaml
  label: Google Drive Files API
  slug: google-drive-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-files-api-openapi.yml
- filename: google-drive-about-api-openapi.yml
  format: yaml
  label: Google Drive About API
  slug: google-drive-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-about-api-openapi.yml
- filename: google-drive-accessproposals-api-openapi.yml
  format: yaml
  label: Google Drive Accessproposals API
  slug: google-drive-accessproposals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-accessproposals-api-openapi.yml
- filename: google-drive-approvals-api-openapi.yml
  format: yaml
  label: Google Drive Approvals API
  slug: google-drive-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-approvals-api-openapi.yml
- filename: google-drive-apps-api-openapi.yml
  format: yaml
  label: Google Drive Apps API
  slug: google-drive-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-apps-api-openapi.yml
- filename: google-drive-changes-api-openapi.yml
  format: yaml
  label: Google Drive Changes API
  slug: google-drive-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-changes-api-openapi.yml
- filename: google-drive-channels-api-openapi.yml
  format: yaml
  label: Google Drive Channels API
  slug: google-drive-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-channels-api-openapi.yml
- filename: google-drive-comments-api-openapi.yml
  format: yaml
  label: Google Drive Comments API
  slug: google-drive-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-comments-api-openapi.yml
- filename: google-drive-drives-api-openapi.yml
  format: yaml
  label: Google Drive Drives API
  slug: google-drive-drives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-drives-api-openapi.yml
- filename: google-drive-operations-api-openapi.yml
  format: yaml
  label: Google Drive Operations API
  slug: google-drive-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-operations-api-openapi.yml
- filename: google-drive-permissions-api-openapi.yml
  format: yaml
  label: Google Drive Permissions API
  slug: google-drive-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-permissions-api-openapi.yml
- filename: google-drive-replies-api-openapi.yml
  format: yaml
  label: Google Drive Replies API
  slug: google-drive-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-replies-api-openapi.yml
- filename: google-drive-revisions-api-openapi.yml
  format: yaml
  label: Google Drive Revisions API
  slug: google-drive-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-revisions-api-openapi.yml
- filename: google-drive-teamdrives-api-openapi.yml
  format: yaml
  label: Google Drive Teamdrives API
  slug: google-drive-teamdrives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-teamdrives-api-openapi.yml
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
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:04 2026 GMT
  host: console.cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Drive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Drive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Drive
provider_slug: google-drive
slug: google-drive-domain-security
source_filename: google-drive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: console.cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-drive/security/google-drive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Storage
- Collaboration
- Document Management
- Drives
- File
- Google
- Storage
---
