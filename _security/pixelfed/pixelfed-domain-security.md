---
api_specs:
- filename: pixelfed-accounts-api-openapi.yml
  format: yaml
  label: Pixelfed Accounts API
  slug: pixelfed-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-accounts-api-openapi.yml
- filename: pixelfed-blocks-and-mutes-api-openapi.yml
  format: yaml
  label: Pixelfed Blocks and Mutes API
  slug: pixelfed-blocks-and-mutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-blocks-and-mutes-api-openapi.yml
- filename: pixelfed-bookmarks-api-openapi.yml
  format: yaml
  label: Pixelfed Bookmarks API
  slug: pixelfed-bookmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-bookmarks-api-openapi.yml
- filename: pixelfed-collections-api-openapi.yml
  format: yaml
  label: Pixelfed Collections API
  slug: pixelfed-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-collections-api-openapi.yml
- filename: pixelfed-direct-messages-api-openapi.yml
  format: yaml
  label: Pixelfed Direct Messages API
  slug: pixelfed-direct-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-direct-messages-api-openapi.yml
- filename: pixelfed-discovery-api-openapi.yml
  format: yaml
  label: Pixelfed Discovery API
  slug: pixelfed-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-discovery-api-openapi.yml
- filename: pixelfed-favourites-api-openapi.yml
  format: yaml
  label: Pixelfed Favourites API
  slug: pixelfed-favourites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-favourites-api-openapi.yml
- filename: pixelfed-follow-requests-api-openapi.yml
  format: yaml
  label: Pixelfed Follow Requests API
  slug: pixelfed-follow-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-follow-requests-api-openapi.yml
- filename: pixelfed-instance-api-openapi.yml
  format: yaml
  label: Pixelfed Instance API
  slug: pixelfed-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-instance-api-openapi.yml
- filename: pixelfed-lists-api-openapi.yml
  format: yaml
  label: Pixelfed Lists API
  slug: pixelfed-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-lists-api-openapi.yml
- filename: pixelfed-media-api-openapi.yml
  format: yaml
  label: Pixelfed Media API
  slug: pixelfed-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-media-api-openapi.yml
- filename: pixelfed-notifications-api-openapi.yml
  format: yaml
  label: Pixelfed Notifications API
  slug: pixelfed-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-notifications-api-openapi.yml
- filename: pixelfed-push-notifications-api-openapi.yml
  format: yaml
  label: Pixelfed Push Notifications API
  slug: pixelfed-push-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-push-notifications-api-openapi.yml
- filename: pixelfed-search-api-openapi.yml
  format: yaml
  label: Pixelfed Search API
  slug: pixelfed-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-search-api-openapi.yml
- filename: pixelfed-statuses-api-openapi.yml
  format: yaml
  label: Pixelfed Statuses API
  slug: pixelfed-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-statuses-api-openapi.yml
- filename: pixelfed-stories-api-openapi.yml
  format: yaml
  label: Pixelfed Stories API
  slug: pixelfed-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-stories-api-openapi.yml
- filename: pixelfed-timelines-api-openapi.yml
  format: yaml
  label: Pixelfed Timelines API
  slug: pixelfed-timelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-timelines-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pixelfed.org
  spf: true
hosts:
- cert_expires: Sep  9 10:17:04 2026 GMT
  host: docs.pixelfed.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixelfed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixelfed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pixelfed
provider_slug: pixelfed
slug: pixelfed-domain-security
source_filename: pixelfed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.pixelfed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:17:04 2026 GMT\n  hsts: false\ndomains:\n- domain: pixelfed.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/security/pixelfed-domain-security.yml
summary_line: TLSv1.3
tags:
- Fediverse
- ActivityPub
- Photo Sharing
- Social-Media
- Open-Source
- Decentralized
- Mastodon Compatible
- Federation
---
