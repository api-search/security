---
api_specs:
- filename: listennotes-directory-api-api-openapi.yml
  format: yaml
  label: Listen Notes Directory API API
  slug: listennotes-directory-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-directory-api-api-openapi.yml
- filename: listennotes-insights-api-api-openapi.yml
  format: yaml
  label: Listen Notes Insights API API
  slug: listennotes-insights-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-insights-api-api-openapi.yml
- filename: listennotes-playlist-api-api-openapi.yml
  format: yaml
  label: Listen Notes Playlist API API
  slug: listennotes-playlist-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-playlist-api-api-openapi.yml
- filename: listennotes-podcaster-api-api-openapi.yml
  format: yaml
  label: Listen Notes Podcaster API API
  slug: listennotes-podcaster-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-podcaster-api-api-openapi.yml
- filename: listennotes-search-api-api-openapi.yml
  format: yaml
  label: Listen Notes Search API API
  slug: listennotes-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-search-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: listennotes.com
  spf: true
hosts:
- cert_expires: Aug 21 16:29:19 2026 GMT
  host: www.listennotes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 16:29:19 2026 GMT
  host: listen-api.listennotes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Listennotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listen Notes, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Listen Notes
provider_slug: listennotes
slug: listennotes-domain-security
source_filename: listennotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.listennotes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:29:19 2026 GMT\n  hsts: false\n- host: listen-api.listennotes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:29:19 2026 GMT\n  hsts: false\ndomains:\n- domain: listennotes.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/security/listennotes-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Podcasts
- Podcast Search
- Podcast Directory
- Search
- Audio
- Media
- Podcast Insights
---
