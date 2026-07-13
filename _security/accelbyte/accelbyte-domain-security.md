---
api_specs:
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte IAM API
  slug: accelbyte-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Basic (Player Profile) API
  slug: accelbyte-basic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Cloud Save API
  slug: accelbyte-cloudsave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Statistics & Leaderboard API
  slug: accelbyte-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Matchmaking API
  slug: accelbyte-matchmaking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Lobby & Session API
  slug: accelbyte-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Commerce (Platform) API
  slug: accelbyte-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Seasons & Battle Pass API
  slug: accelbyte-seasonpass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Achievement API
  slug: accelbyte-achievement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Dedicated Server (Armada/DSMC) API
  slug: accelbyte-dsmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Analytics & Telemetry API
  slug: accelbyte-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte UGC API
  slug: accelbyte-ugc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: accelbyte.io
  spf: true
hosts:
- cert_expires: Sep 17 04:03:55 2026 GMT
  host: accelbyte.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: docs.accelbyte.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: demo.accelbyte.io
  https: false
kind: domain-security
layout: security
method: probed
name: Accelbyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AccelByte, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AccelByte
provider_slug: accelbyte
slug: accelbyte-domain-security
source_filename: accelbyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accelbyte.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 04:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.accelbyte.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\n- host: demo.accelbyte.io\n  https: false\ndomains:\n- domain: accelbyte.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/security/accelbyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Backend
- BaaS
- Live Services
- Player Accounts
- Commerce
---
