---
api_specs:
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Meetings API
  slug: meetings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Participants API
  slug: participants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Sessions API
  slug: sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Recordings API
  slug: recordings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Livestreams API
  slug: livestreams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dyte.io
  spf: true
hosts:
- cert_expires: Aug 29 05:39:05 2026 GMT
  host: dyte.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 17:57:05 2026 GMT
  host: docs.dyte.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 18:14:33 2026 GMT
  host: api.dyte.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dyte, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dyte
provider_slug: dyte
slug: dyte-domain-security
source_filename: dyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dyte.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:39:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dyte.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 17:57:05 2026 GMT\n  hsts: false\n- host: api.dyte.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 18:14:33 2026 GMT\n  hsts: null\ndomains:\n- domain: dyte.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/security/dyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Voice
- Real Time
- WebRTC
- SDK
- Communications
---
