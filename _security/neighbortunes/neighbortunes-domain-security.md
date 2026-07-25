---
api_specs:
- filename: neighbortunes-albums-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Albums.{format} API
  slug: neighbortunes-albums-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-albums-format-api-openapi.yml
- filename: neighbortunes-appearances-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Appearances.{format} API
  slug: neighbortunes-appearances-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-appearances-format-api-openapi.yml
- filename: neighbortunes-jamcharts-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Jamcharts.{format} API
  slug: neighbortunes-jamcharts-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-jamcharts-format-api-openapi.yml
- filename: neighbortunes-latest-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Latest.{format} API
  slug: neighbortunes-latest-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-latest-format-api-openapi.yml
- filename: neighbortunes-links-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Links.{format} API
  slug: neighbortunes-links-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-links-format-api-openapi.yml
- filename: neighbortunes-list-api-openapi.yml
  format: yaml
  label: Neighbortunes List API
  slug: neighbortunes-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-list-api-openapi.yml
- filename: neighbortunes-metadata-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Metadata.{format} API
  slug: neighbortunes-metadata-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-metadata-format-api-openapi.yml
- filename: neighbortunes-setlists-api-openapi.yml
  format: yaml
  label: Neighbortunes Setlists API
  slug: neighbortunes-setlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-setlists-api-openapi.yml
- filename: neighbortunes-setlists-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Setlists.{format} API
  slug: neighbortunes-setlists-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-setlists-format-api-openapi.yml
- filename: neighbortunes-shows-api-openapi.yml
  format: yaml
  label: Neighbortunes Shows API
  slug: neighbortunes-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-shows-api-openapi.yml
- filename: neighbortunes-shows-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Shows.{format} API
  slug: neighbortunes-shows-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-shows-format-api-openapi.yml
- filename: neighbortunes-songs-api-openapi.yml
  format: yaml
  label: Neighbortunes Songs API
  slug: neighbortunes-songs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-songs-api-openapi.yml
- filename: neighbortunes-songs-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Songs.{format} API
  slug: neighbortunes-songs-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-songs-format-api-openapi.yml
- filename: neighbortunes-uploads-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Uploads.{format} API
  slug: neighbortunes-uploads-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-uploads-format-api-openapi.yml
- filename: neighbortunes-venues-api-openapi.yml
  format: yaml
  label: Neighbortunes Venues API
  slug: neighbortunes-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-venues-api-openapi.yml
- filename: neighbortunes-venues-format-api-openapi.yml
  format: yaml
  label: Neighbortunes Venues.{format} API
  slug: neighbortunes-venues-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/openapi/neighbortunes-venues-format-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: neighbortunes.net
  spf: true
hosts:
- cert_expires: Sep  1 04:18:10 2026 GMT
  host: www.neighbortunes.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:18:10 2026 GMT
  host: neighbortunes.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neighbortunes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neighbortunes, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Neighbortunes
provider_slug: neighbortunes
slug: neighbortunes-domain-security
source_filename: neighbortunes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neighbortunes.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:18:10 2026 GMT\n  hsts: false\n- host: neighbortunes.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:18:10 2026 GMT\n  hsts: false\ndomains:\n- domain: neighbortunes.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neighbortunes/refs/heads/main/security/neighbortunes-domain-security.yml
summary_line: TLSv1.3
tags:
- Music
- Setlists
- Fan Site
---
