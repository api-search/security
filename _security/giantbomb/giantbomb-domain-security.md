---
api_specs:
- filename: giantbomb-characters-api-openapi.yml
  format: yaml
  label: Giant Bomb Characters API
  slug: giantbomb-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-characters-api-openapi.yml
- filename: giantbomb-companies-api-openapi.yml
  format: yaml
  label: Giant Bomb Companies API
  slug: giantbomb-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-companies-api-openapi.yml
- filename: giantbomb-franchises-api-openapi.yml
  format: yaml
  label: Giant Bomb Franchises API
  slug: giantbomb-franchises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-franchises-api-openapi.yml
- filename: giantbomb-games-api-openapi.yml
  format: yaml
  label: Giant Bomb Games API
  slug: giantbomb-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-games-api-openapi.yml
- filename: giantbomb-platforms-api-openapi.yml
  format: yaml
  label: Giant Bomb Platforms API
  slug: giantbomb-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-platforms-api-openapi.yml
- filename: giantbomb-releases-api-openapi.yml
  format: yaml
  label: Giant Bomb Releases API
  slug: giantbomb-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-releases-api-openapi.yml
- filename: giantbomb-reviews-api-openapi.yml
  format: yaml
  label: Giant Bomb Reviews API
  slug: giantbomb-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-reviews-api-openapi.yml
- filename: giantbomb-search-api-openapi.yml
  format: yaml
  label: Giant Bomb Search API
  slug: giantbomb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-search-api-openapi.yml
- filename: giantbomb-videos-api-openapi.yml
  format: yaml
  label: Giant Bomb Videos API
  slug: giantbomb-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: giantbomb.com
  spf: true
hosts:
- cert_expires: Aug 26 00:14:39 2026 GMT
  host: www.giantbomb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Giantbomb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Giant Bomb, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Giant Bomb
provider_slug: giantbomb
slug: giantbomb-domain-security
source_filename: giantbomb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.giantbomb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:14:39 2026 GMT\n  hsts: null\ndomains:\n- domain: giantbomb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/security/giantbomb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Entertainment
- Video Games
- Game Database
- Gaming
- Media
---
