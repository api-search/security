---
api_specs:
- filename: podcastindex-add-api-openapi.yml
  format: yaml
  label: PodcastIndex Add API
  slug: podcastindex-add-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-add-api-openapi.yml
- filename: podcastindex-apple-replacement-api-openapi.yml
  format: yaml
  label: PodcastIndex Apple Replacement API
  slug: podcastindex-apple-replacement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-apple-replacement-api-openapi.yml
- filename: podcastindex-categories-api-openapi.yml
  format: yaml
  label: PodcastIndex Categories API
  slug: podcastindex-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-categories-api-openapi.yml
- filename: podcastindex-episodes-api-openapi.yml
  format: yaml
  label: PodcastIndex Episodes API
  slug: podcastindex-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-episodes-api-openapi.yml
- filename: podcastindex-hub-api-openapi.yml
  format: yaml
  label: PodcastIndex Hub API
  slug: podcastindex-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-hub-api-openapi.yml
- filename: podcastindex-podcasts-api-openapi.yml
  format: yaml
  label: PodcastIndex Podcasts API
  slug: podcastindex-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-podcasts-api-openapi.yml
- filename: podcastindex-recent-api-openapi.yml
  format: yaml
  label: PodcastIndex Recent API
  slug: podcastindex-recent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-recent-api-openapi.yml
- filename: podcastindex-search-api-openapi.yml
  format: yaml
  label: PodcastIndex Search API
  slug: podcastindex-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-search-api-openapi.yml
- filename: podcastindex-static-data-api-openapi.yml
  format: yaml
  label: PodcastIndex Static Data API
  slug: podcastindex-static-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-static-data-api-openapi.yml
- filename: podcastindex-stats-api-openapi.yml
  format: yaml
  label: PodcastIndex Stats API
  slug: podcastindex-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-stats-api-openapi.yml
- filename: podcastindex-value-api-openapi.yml
  format: yaml
  label: PodcastIndex Value API
  slug: podcastindex-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-value-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: podcastindex.org
  spf: true
hosts:
- cert_expires: Aug 18 15:12:09 2026 GMT
  host: podcastindex.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 15:12:09 2026 GMT
  host: api.podcastindex.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podcastindex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PodcastIndex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PodcastIndex
provider_slug: podcastindex
slug: podcastindex-domain-security
source_filename: podcastindex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podcastindex.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:12:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.podcastindex.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:12:09 2026 GMT\n  hsts: false\ndomains:\n- domain: podcastindex.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/security/podcastindex-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Podcasting
- Podcast Index
- Discovery
- Open Data
---
