---
api_specs:
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Media API
  slug: yodeck-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Playlists API
  slug: yodeck-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Layouts API
  slug: yodeck-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Screens API
  slug: yodeck-screens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Schedules API
  slug: yodeck-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Shows API
  slug: yodeck-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Workspaces API
  slug: yodeck-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yodeck.com
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: www.yodeck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: app.yodeck.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yodeck Signage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yodeck, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yodeck
provider_slug: yodeck-signage
slug: yodeck-signage-domain-security
source_filename: yodeck-signage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yodeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.yodeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: yodeck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/security/yodeck-signage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Signage
- Screen Management
- Content Management
- Media
- Playlists
- Scheduling
- Raspberry Pi
---
