---
api_specs:
- filename: discourse-admin-api-openapi.yml
  format: yaml
  label: Discourse Admin API
  slug: discourse-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-admin-api-openapi.yml
- filename: discourse-backups-api-openapi.yml
  format: yaml
  label: Discourse Backups API
  slug: discourse-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-backups-api-openapi.yml
- filename: discourse-badges-api-openapi.yml
  format: yaml
  label: Discourse Badges API
  slug: discourse-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-badges-api-openapi.yml
- filename: discourse-categories-api-openapi.yml
  format: yaml
  label: Discourse Categories API
  slug: discourse-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-categories-api-openapi.yml
- filename: discourse-discourse-calendar-events-api-openapi.yml
  format: yaml
  label: Discourse Discourse Calendar - Events API
  slug: discourse-discourse-calendar-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-discourse-calendar-events-api-openapi.yml
- filename: discourse-groups-api-openapi.yml
  format: yaml
  label: Discourse Groups API
  slug: discourse-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-groups-api-openapi.yml
- filename: discourse-invites-api-openapi.yml
  format: yaml
  label: Discourse Invites API
  slug: discourse-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-invites-api-openapi.yml
- filename: discourse-notifications-api-openapi.yml
  format: yaml
  label: Discourse Notifications API
  slug: discourse-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-notifications-api-openapi.yml
- filename: discourse-posts-api-openapi.yml
  format: yaml
  label: Discourse Posts API
  slug: discourse-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-posts-api-openapi.yml
- filename: discourse-private-messages-api-openapi.yml
  format: yaml
  label: Discourse Private Messages API
  slug: discourse-private-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-private-messages-api-openapi.yml
- filename: discourse-search-api-openapi.yml
  format: yaml
  label: Discourse Search API
  slug: discourse-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-search-api-openapi.yml
- filename: discourse-site-api-openapi.yml
  format: yaml
  label: Discourse Site API
  slug: discourse-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-site-api-openapi.yml
- filename: discourse-tags-api-openapi.yml
  format: yaml
  label: Discourse Tags API
  slug: discourse-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-tags-api-openapi.yml
- filename: discourse-topics-api-openapi.yml
  format: yaml
  label: Discourse Topics API
  slug: discourse-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-topics-api-openapi.yml
- filename: discourse-uploads-api-openapi.yml
  format: yaml
  label: Discourse Uploads API
  slug: discourse-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-uploads-api-openapi.yml
- filename: discourse-users-api-openapi.yml
  format: yaml
  label: Discourse Users API
  slug: discourse-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: discourse.org
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.discourse.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 00:02:48 2026 GMT
  host: meta.discourse.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Discourse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Discourse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Discourse
provider_slug: discourse
slug: discourse-domain-security
source_filename: discourse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.discourse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: meta.discourse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:02:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: discourse.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/security/discourse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communities
- Forums
- Open Source
---
