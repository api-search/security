---
api_specs:
- filename: umami-authentication-api-openapi.yml
  format: yaml
  label: Umami Authentication API
  slug: umami-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-authentication-api-openapi.yml
- filename: umami-events-api-openapi.yml
  format: yaml
  label: Umami Events API
  slug: umami-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-events-api-openapi.yml
- filename: umami-sessions-api-openapi.yml
  format: yaml
  label: Umami Sessions API
  slug: umami-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-sessions-api-openapi.yml
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
- filename: umami-website-statistics-api-openapi.yml
  format: yaml
  label: Umami Website Statistics API
  slug: umami-website-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-website-statistics-api-openapi.yml
- filename: umami-websites-api-openapi.yml
  format: yaml
  label: Umami Websites API
  slug: umami-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-websites-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: umami.is
  spf: true
hosts:
- cert_expires: Nov  6 18:17:14 2026 GMT
  host: umami.is
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:58:42 2026 GMT
  host: api.umami.is
  hsts: null
  https: true
  tls_version: TLSv1.3
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
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: umami.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 18:17:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.umami.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:58:42 2026 GMT\n  hsts: null\ndomains:\n- domain: umami.is\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/security/umami-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cookieless Tracking
- Open-Source
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
