---
api_specs:
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Content API
  slug: ghost-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Posts API
  slug: ghost-admin-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Pages API
  slug: ghost-admin-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Members API
  slug: ghost-admin-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Tags and Labels API
  slug: ghost-admin-tags-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Tiers and Offers API
  slug: ghost-admin-tiers-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Newsletters API
  slug: ghost-admin-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Users and Site API
  slug: ghost-admin-users-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Media and Themes API
  slug: ghost-admin-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Webhooks API
  slug: ghost-admin-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
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
name: Ghost Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ghost, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ghost
provider_slug: ghost-org
slug: ghost-org-domain-security
source_filename: ghost-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ghost.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ghost.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:18:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ghost.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/security/ghost-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Publishing
- Newsletters
- Memberships
- Subscriptions
- CMS
- Open Source
- Content
---
