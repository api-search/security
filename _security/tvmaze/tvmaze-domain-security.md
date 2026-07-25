---
api_specs:
- filename: tvmaze-auth-api-openapi.yml
  format: yaml
  label: TVmaze auth API
  slug: tvmaze-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-auth-api-openapi.yml
- filename: tvmaze-episodes-api-openapi.yml
  format: yaml
  label: TVmaze Episodes API
  slug: tvmaze-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-episodes-api-openapi.yml
- filename: tvmaze-followed-networks-api-openapi.yml
  format: yaml
  label: TVmaze followed networks API
  slug: tvmaze-followed-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-followed-networks-api-openapi.yml
- filename: tvmaze-followed-people-api-openapi.yml
  format: yaml
  label: TVmaze followed people API
  slug: tvmaze-followed-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-followed-people-api-openapi.yml
- filename: tvmaze-followed-shows-api-openapi.yml
  format: yaml
  label: TVmaze followed shows API
  slug: tvmaze-followed-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-followed-shows-api-openapi.yml
- filename: tvmaze-followed-webchannels-api-openapi.yml
  format: yaml
  label: TVmaze followed webchannels API
  slug: tvmaze-followed-webchannels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-followed-webchannels-api-openapi.yml
- filename: tvmaze-marked-episodes-api-openapi.yml
  format: yaml
  label: TVmaze marked episodes API
  slug: tvmaze-marked-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-marked-episodes-api-openapi.yml
- filename: tvmaze-people-api-openapi.yml
  format: yaml
  label: TVmaze People API
  slug: tvmaze-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-people-api-openapi.yml
- filename: tvmaze-schedule-api-openapi.yml
  format: yaml
  label: TVmaze Schedule API
  slug: tvmaze-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-schedule-api-openapi.yml
- filename: tvmaze-scrobbling-api-openapi.yml
  format: yaml
  label: TVmaze scrobbling API
  slug: tvmaze-scrobbling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-scrobbling-api-openapi.yml
- filename: tvmaze-search-api-openapi.yml
  format: yaml
  label: TVmaze Search API
  slug: tvmaze-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-search-api-openapi.yml
- filename: tvmaze-seasons-api-openapi.yml
  format: yaml
  label: TVmaze Seasons API
  slug: tvmaze-seasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-seasons-api-openapi.yml
- filename: tvmaze-shows-api-openapi.yml
  format: yaml
  label: TVmaze Shows API
  slug: tvmaze-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-shows-api-openapi.yml
- filename: tvmaze-tagged-shows-api-openapi.yml
  format: yaml
  label: TVmaze tagged shows API
  slug: tvmaze-tagged-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-tagged-shows-api-openapi.yml
- filename: tvmaze-updates-api-openapi.yml
  format: yaml
  label: TVmaze Updates API
  slug: tvmaze-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-updates-api-openapi.yml
- filename: tvmaze-voted-episodes-api-openapi.yml
  format: yaml
  label: TVmaze voted episodes API
  slug: tvmaze-voted-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-voted-episodes-api-openapi.yml
- filename: tvmaze-voted-shows-api-openapi.yml
  format: yaml
  label: TVmaze voted shows API
  slug: tvmaze-voted-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-voted-shows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tvmaze.com
  spf: true
hosts:
- cert_expires: Sep  8 15:28:36 2026 GMT
  host: www.tvmaze.com
  hsts: true
  hsts_max_age: 2629800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 15:28:36 2026 GMT
  host: api.tvmaze.com
  hsts: true
  hsts_max_age: 2629800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 19:13:19 2026 GMT
  host: static.tvmaze.com
  hsts: true
  hsts_max_age: 2629800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tvmaze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TVmaze, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TVmaze
provider_slug: tvmaze
slug: tvmaze-domain-security
source_filename: tvmaze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tvmaze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:28:36 2026 GMT\n  hsts: true\n  hsts_max_age: 2629800\n- host: api.tvmaze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:28:36 2026 GMT\n  hsts: true\n  hsts_max_age: 2629800\n- host: static.tvmaze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 2629800\ndomains:\n- domain: tvmaze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/security/tvmaze-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Video
- Television
- Streaming
- Schedule
- Metadata
- Entertainment
- Public APIs
---
