---
api_specs:
- filename: ghost-authors-api-openapi.yml
  format: yaml
  label: Ghost Authors API
  slug: ghost-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-authors-api-openapi.yml
- filename: ghost-images-api-openapi.yml
  format: yaml
  label: Ghost Images API
  slug: ghost-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-images-api-openapi.yml
- filename: ghost-members-api-openapi.yml
  format: yaml
  label: Ghost Members API
  slug: ghost-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-members-api-openapi.yml
- filename: ghost-newsletters-api-openapi.yml
  format: yaml
  label: Ghost Newsletters API
  slug: ghost-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-newsletters-api-openapi.yml
- filename: ghost-offers-api-openapi.yml
  format: yaml
  label: Ghost Offers API
  slug: ghost-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-offers-api-openapi.yml
- filename: ghost-pages-api-openapi.yml
  format: yaml
  label: Ghost Pages API
  slug: ghost-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-pages-api-openapi.yml
- filename: ghost-posts-api-openapi.yml
  format: yaml
  label: Ghost Posts API
  slug: ghost-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-posts-api-openapi.yml
- filename: ghost-settings-api-openapi.yml
  format: yaml
  label: Ghost Settings API
  slug: ghost-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-settings-api-openapi.yml
- filename: ghost-site-api-openapi.yml
  format: yaml
  label: Ghost Site API
  slug: ghost-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-site-api-openapi.yml
- filename: ghost-tags-api-openapi.yml
  format: yaml
  label: Ghost Tags API
  slug: ghost-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-tags-api-openapi.yml
- filename: ghost-themes-api-openapi.yml
  format: yaml
  label: Ghost Themes API
  slug: ghost-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-themes-api-openapi.yml
- filename: ghost-tiers-api-openapi.yml
  format: yaml
  label: Ghost Tiers API
  slug: ghost-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-tiers-api-openapi.yml
- filename: ghost-users-api-openapi.yml
  format: yaml
  label: Ghost Users API
  slug: ghost-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-users-api-openapi.yml
- filename: ghost-webhooks-api-openapi.yml
  format: yaml
  label: Ghost Webhooks API
  slug: ghost-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ghost.org
  spf: true
hosts:
- cert_expires: Sep 23 21:23:50 2026 GMT
  host: ghost.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:18:17 2026 GMT
  host: docs.ghost.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ghost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ghost, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ghost
provider_slug: ghost
slug: ghost-domain-security
source_filename: ghost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ghost.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ghost.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:18:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ghost.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/security/ghost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Publishing
- Newsletters
- Memberships
- Content
- Open Source
---
