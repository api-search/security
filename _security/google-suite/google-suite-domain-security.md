---
api_specs:
- filename: rest
  format: yaml
  label: Gmail API
  slug: gmail-api
  spec_type: OpenAPI
  url: https://gmail.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Calendar API
  slug: google-calendar-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/calendar/v3/rest
- filename: rest
  format: yaml
  label: Google Drive API
  slug: google-drive-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/drive/v3/rest
- filename: rest
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://docs.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://sheets.googleapis.com/$discovery/rest?version=v4
- filename: rest
  format: yaml
  label: Google Slides API
  slug: google-slides-api
  spec_type: OpenAPI
  url: https://slides.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Chat API
  slug: google-chat-api
  spec_type: OpenAPI
  url: https://chat.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Admin SDK
  slug: google-admin-sdk
  spec_type: OpenAPI
  url: https://admin.googleapis.com/$discovery/rest?version=directory_v1
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
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: gmail.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: www.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Suite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Workspace (G Suite), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Workspace (G Suite)
provider_slug: google-suite
slug: google-suite-domain-security
source_filename: google-suite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gmail.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: www.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suite/refs/heads/main/security/google-suite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Collaboration
- Enterprise
- Google
- Productivity
- Workspace
---
