---
api_specs:
- filename: meet-conference-records-api-openapi.yml
  format: yaml
  label: Google Meet Conference Records API
  slug: meet-conference-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meet/refs/heads/main/openapi/meet-conference-records-api-openapi.yml
- filename: meet-participants-api-openapi.yml
  format: yaml
  label: Google Meet Participants API
  slug: meet-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meet/refs/heads/main/openapi/meet-participants-api-openapi.yml
- filename: meet-recordings-api-openapi.yml
  format: yaml
  label: Google Meet Recordings API
  slug: meet-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meet/refs/heads/main/openapi/meet-recordings-api-openapi.yml
- filename: meet-spaces-api-openapi.yml
  format: yaml
  label: Google Meet Spaces API
  slug: meet-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meet/refs/heads/main/openapi/meet-spaces-api-openapi.yml
- filename: meet-transcripts-api-openapi.yml
  format: yaml
  label: Google Meet Transcripts API
  slug: meet-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meet/refs/heads/main/openapi/meet-transcripts-api-openapi.yml
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
  host: meet.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: meet.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Meet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Meet
provider_slug: meet
slug: meet-domain-security
source_filename: meet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meet.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: meet.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meet/refs/heads/main/security/meet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video Conferencing
- Meetings
- Communications
- Collaboration
- Google Workspace
- Recordings
- Transcripts
---
