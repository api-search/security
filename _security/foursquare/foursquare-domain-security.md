---
api_specs:
- filename: foursquare-ask-api-openapi.yml
  format: yaml
  label: Foursquare Ask API
  slug: foursquare-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-ask-api-openapi.yml
- filename: foursquare-autocomplete-api-openapi.yml
  format: yaml
  label: Foursquare Autocomplete API
  slug: foursquare-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-autocomplete-api-openapi.yml
- filename: foursquare-details-api-openapi.yml
  format: yaml
  label: Foursquare Details API
  slug: foursquare-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-details-api-openapi.yml
- filename: foursquare-geotagging-api-openapi.yml
  format: yaml
  label: Foursquare Geotagging API
  slug: foursquare-geotagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-geotagging-api-openapi.yml
- filename: foursquare-match-api-openapi.yml
  format: yaml
  label: Foursquare Match API
  slug: foursquare-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-match-api-openapi.yml
- filename: foursquare-photos-api-openapi.yml
  format: yaml
  label: Foursquare Photos API
  slug: foursquare-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-photos-api-openapi.yml
- filename: foursquare-search-api-openapi.yml
  format: yaml
  label: Foursquare Search API
  slug: foursquare-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-search-api-openapi.yml
- filename: foursquare-tips-api-openapi.yml
  format: yaml
  label: Foursquare Tips API
  slug: foursquare-tips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-tips-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: foursquare.com
  spf: true
hosts:
- cert_expires: Sep 16 22:33:04 2026 GMT
  host: foursquare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:31:51 2026 GMT
  host: docs.foursquare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 22:33:04 2026 GMT
  host: places-api.foursquare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Foursquare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foursquare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Foursquare
provider_slug: foursquare
slug: foursquare-domain-security
source_filename: foursquare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foursquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:33:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.foursquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:31:51 2026 GMT\n  hsts: null\n- host: places-api.foursquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:33:04 2026 GMT\n  hsts: null\ndomains:\n- domain: foursquare.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/security/foursquare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Locations
- Places
- Geocoding
- Recommendations
- Reviews
- Movement
---
