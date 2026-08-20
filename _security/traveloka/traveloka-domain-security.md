---
api_specs:
- filename: traveloka-1-1-content-hotel-room-api-openapi.yml
  format: yaml
  label: Traveloka 1.1 Content - Hotel & Room API
  slug: traveloka-1-1-content-hotel-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-1-1-content-hotel-room-api-openapi.yml
- filename: traveloka-2-1-search-hotellist-api-openapi.yml
  format: yaml
  label: Traveloka 2.1 Search - HotelList API
  slug: traveloka-2-1-search-hotellist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-2-1-search-hotellist-api-openapi.yml
- filename: traveloka-2-2-search-roomlist-api-openapi.yml
  format: yaml
  label: Traveloka 2.2 Search - RoomList API
  slug: traveloka-2-2-search-roomlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-2-2-search-roomlist-api-openapi.yml
- filename: traveloka-2-3-search-bulkroomlist-api-openapi.yml
  format: yaml
  label: Traveloka 2.3 Search - BulkRoomList API
  slug: traveloka-2-3-search-bulkroomlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-2-3-search-bulkroomlist-api-openapi.yml
- filename: traveloka-3-1-booking-book-api-openapi.yml
  format: yaml
  label: Traveloka 3.1 Booking - Book API
  slug: traveloka-3-1-booking-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-1-booking-book-api-openapi.yml
- filename: traveloka-3-2-booking-issuecheck-api-openapi.yml
  format: yaml
  label: Traveloka 3.2 Booking - IssueCheck API
  slug: traveloka-3-2-booking-issuecheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-2-booking-issuecheck-api-openapi.yml
- filename: traveloka-3-3-booking-issue-api-openapi.yml
  format: yaml
  label: Traveloka 3.3 Booking - Issue API
  slug: traveloka-3-3-booking-issue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-3-booking-issue-api-openapi.yml
- filename: traveloka-3-4-booking-bookingsummary-api-openapi.yml
  format: yaml
  label: Traveloka 3.4 Booking - BookingSummary API
  slug: traveloka-3-4-booking-bookingsummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-4-booking-bookingsummary-api-openapi.yml
- filename: traveloka-3-5-booking-cancel-api-openapi.yml
  format: yaml
  label: Traveloka 3.5 Booking - Cancel API
  slug: traveloka-3-5-booking-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-5-booking-cancel-api-openapi.yml
- filename: traveloka-authorization-api-openapi.yml
  format: yaml
  label: Traveloka Authorization API
  slug: traveloka-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-authorization-api-openapi.yml
- filename: traveloka-booking-api-openapi.yml
  format: yaml
  label: Traveloka Booking API
  slug: traveloka-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-booking-api-openapi.yml
- filename: traveloka-content-api-openapi.yml
  format: yaml
  label: Traveloka Content API
  slug: traveloka-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-content-api-openapi.yml
- filename: traveloka-discovery-optional-api-openapi.yml
  format: yaml
  label: Traveloka Discovery (Optional) API
  slug: traveloka-discovery-optional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-discovery-optional-api-openapi.yml
- filename: traveloka-rate-api-openapi.yml
  format: yaml
  label: Traveloka Rate API
  slug: traveloka-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-rate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: traveloka.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: travelokapartnersnetwork.com
  spf: false
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.traveloka.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: developer.travelokapartnersnetwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.travelokapartnersnetwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Traveloka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traveloka, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Traveloka
provider_slug: traveloka
slug: traveloka-domain-security
source_filename: traveloka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.traveloka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n- host: developer.travelokapartnersnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.travelokapartnersnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: traveloka.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: travelokapartnersnetwork.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/security/traveloka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Online Travel Agency
- Accommodation
- Hotel Booking
- Flights
- Activities
- Hospitality
- Distribution
- Channel Manager
- OpenTravel
- Southeast Asia
- Indonesia
---
