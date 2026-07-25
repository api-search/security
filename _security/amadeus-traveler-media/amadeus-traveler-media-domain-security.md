---
api_specs:
- filename: amadeus-traveler-media-category-rated-areas-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media category-rated-areas API
  slug: amadeus-traveler-media-category-rated-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-category-rated-areas-api-openapi.yml
- filename: amadeus-traveler-media-hotel-ratings-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media Hotel Ratings API
  slug: amadeus-traveler-media-hotel-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-hotel-ratings-api-openapi.yml
- filename: amadeus-traveler-media-recommended-locations-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media recommended-locations API
  slug: amadeus-traveler-media-recommended-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-recommended-locations-api-openapi.yml
- filename: amadeus-traveler-media-retrieve-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media Retrieve API
  slug: amadeus-traveler-media-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-retrieve-api-openapi.yml
- filename: amadeus-traveler-media-search-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media Search API
  slug: amadeus-traveler-media-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amadeus.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developers.amadeus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 23:59:59 2026 GMT
  host: test.api.amadeus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amadeus Traveler Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amadeus Traveler Media, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
slug: amadeus-traveler-media-domain-security
source_filename: amadeus-traveler-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.amadeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: test.api.amadeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amadeus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/security/amadeus-traveler-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
---
