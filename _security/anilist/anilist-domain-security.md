---
api_specs:
- filename: anilist-openapi.yml
  format: yaml
  label: AniList GraphQL API v2
  slug: anilist-graphql-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anilist/refs/heads/main/openapi/anilist-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anilist.co
  spf: true
hosts:
- cert_expires: Oct  8 17:08:32 2026 GMT
  host: anilist.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 05:02:38 2026 GMT
  host: docs.anilist.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 17:08:32 2026 GMT
  host: graphql.anilist.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anilist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AniList, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AniList
provider_slug: anilist
slug: anilist-domain-security
source_filename: anilist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anilist.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:08:32 2026 GMT\n  hsts: false\n- host: docs.anilist.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:02:38 2026 GMT\n  hsts: false\n- host: graphql.anilist.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:08:32 2026 GMT\n  hsts: null\ndomains:\n- domain: anilist.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anilist/refs/heads/main/security/anilist-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Anime
- Manga
- Entertainment
- Media
- Social
- Database
- GraphQL
- OAuth2
- Public APIs
---
