---
api_specs:
- filename: rottentomatoes-detailed-info-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Detailed Info API
  slug: rottentomatoes-detailed-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-detailed-info-api-openapi.yml
- filename: rottentomatoes-dvd-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes DVD Lists API
  slug: rottentomatoes-dvd-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-dvd-lists-api-openapi.yml
- filename: rottentomatoes-movie-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Movie Lists API
  slug: rottentomatoes-movie-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-movie-lists-api-openapi.yml
- filename: rottentomatoes-search-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Search API
  slug: rottentomatoes-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-search-api-openapi.yml
- filename: rottentomatoes-top-level-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Top Level Lists API
  slug: rottentomatoes-top-level-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-top-level-lists-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fandango.com
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rottentomatoes.com
  spf: true
hosts:
- host: developer.fandango.com
  https: false
- host: api.rottentomatoes.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rottentomatoes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rotten Tomatoes, probed live across 2 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rotten Tomatoes
provider_slug: rottentomatoes
slug: rottentomatoes-domain-security
source_filename: rottentomatoes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.fandango.com\n  https: false\n- host: api.rottentomatoes.com\n  https: false\ndomains:\n- domain: fandango.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rottentomatoes.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/security/rottentomatoes-domain-security.yml
summary_line: DMARC
tags:
- Movies
- Television
- Reviews
- Ratings
- Tomatometer
- Audience Score
- Entertainment
- Media
---
