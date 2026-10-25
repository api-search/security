---
api_specs:
- filename: umami-authentication-api-openapi.yml
  format: yaml
  label: Umami Authentication API
  slug: umami-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-authentication-api-openapi.yml
- filename: umami-teams-api-openapi.yml
  format: yaml
  label: Umami Teams API
  slug: umami-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-teams-api-openapi.yml
- filename: umami-users-api-openapi.yml
  format: yaml
  label: Umami Users API
  slug: umami-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-users-api-openapi.yml
- filename: umami-websites-api-openapi.yml
  format: yaml
  label: Umami Websites API
  slug: umami-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-websites-api-openapi.yml
- filename: umami-account-api-openapi.yml
  format: yaml
  label: Umami Account API
  slug: umami-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-account-api-openapi.yml
- filename: umami-administration-api-openapi.yml
  format: yaml
  label: Umami Administration API
  slug: umami-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-administration-api-openapi.yml
- filename: umami-boards-api-openapi.yml
  format: yaml
  label: Umami Boards API
  slug: umami-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-boards-api-openapi.yml
- filename: umami-collection-api-openapi.yml
  format: yaml
  label: Umami Collection API
  slug: umami-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-collection-api-openapi.yml
- filename: umami-dashboard-api-openapi.yml
  format: yaml
  label: Umami Dashboard API
  slug: umami-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-dashboard-api-openapi.yml
- filename: umami-links-api-openapi.yml
  format: yaml
  label: Umami Links API
  slug: umami-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-links-api-openapi.yml
- filename: umami-pixels-api-openapi.yml
  format: yaml
  label: Umami Pixels API
  slug: umami-pixels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-pixels-api-openapi.yml
- filename: umami-realtime-api-openapi.yml
  format: yaml
  label: Umami Realtime API
  slug: umami-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-realtime-api-openapi.yml
- filename: umami-scripts-api-openapi.yml
  format: yaml
  label: Umami Scripts API
  slug: umami-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-scripts-api-openapi.yml
- filename: umami-shares-api-openapi.yml
  format: yaml
  label: Umami Shares API
  slug: umami-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-shares-api-openapi.yml
- filename: umami-system-api-openapi.yml
  format: yaml
  label: Umami System API
  slug: umami-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-system-api-openapi.yml
- filename: umami-two-factor-authentication-api-openapi.yml
  format: yaml
  label: Umami Two-factor authentication API
  slug: umami-two-factor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-two-factor-authentication-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: umami.is
  spf: true
hosts:
- cert_expires: Jan 16 03:10:04 2027 GMT
  host: umami.is
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 01:34:56 2027 GMT
  host: api.umami.is
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Umami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umami, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Umami
provider_slug: umami
slug: umami-domain-security
source_filename: umami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: umami.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 03:10:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.umami.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 01:34:56 2027 GMT\n  hsts: null\ndomains:\n- domain: umami.is\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/security/umami-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cookieless Tracking
- Open Source
- Privacy
- Web Analytics
- Website Analytics
- Product Analytics
- Event Tracking
- Self-Hosted
- GDPR
- Session Replay
- Heatmaps
- Marketing Attribution
---
