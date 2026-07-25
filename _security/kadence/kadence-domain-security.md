---
api_specs:
- filename: kadence-bookable-day-api-openapi.yml
  format: yaml
  label: Kadence Bookable Day API
  slug: kadence-bookable-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-day-api-openapi.yml
- filename: kadence-bookable-onsite-pass-api-openapi.yml
  format: yaml
  label: Kadence Bookable Onsite Pass API
  slug: kadence-bookable-onsite-pass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-onsite-pass-api-openapi.yml
- filename: kadence-bookable-space-api-openapi.yml
  format: yaml
  label: Kadence Bookable Space API
  slug: kadence-bookable-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-space-api-openapi.yml
- filename: kadence-booking-api-openapi.yml
  format: yaml
  label: Kadence Booking API
  slug: kadence-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-booking-api-openapi.yml
- filename: kadence-building-api-openapi.yml
  format: yaml
  label: Kadence Building API
  slug: kadence-building-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-building-api-openapi.yml
- filename: kadence-floor-api-openapi.yml
  format: yaml
  label: Kadence Floor API
  slug: kadence-floor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-floor-api-openapi.yml
- filename: kadence-neighborhood-api-openapi.yml
  format: yaml
  label: Kadence Neighborhood API
  slug: kadence-neighborhood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-neighborhood-api-openapi.yml
- filename: kadence-space-api-openapi.yml
  format: yaml
  label: Kadence Space API
  slug: kadence-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-space-api-openapi.yml
- filename: kadence-user-api-openapi.yml
  format: yaml
  label: Kadence User API
  slug: kadence-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-user-api-openapi.yml
- filename: kadence-visit-api-openapi.yml
  format: yaml
  label: Kadence Visit API
  slug: kadence-visit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-visit-api-openapi.yml
- filename: kadence-visitor-api-openapi.yml
  format: yaml
  label: Kadence Visitor API
  slug: kadence-visitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-visitor-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kadence.co
  spf: true
- caa:
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onkadence.co
  spf: true
hosts:
- cert_expires: Sep  1 00:06:02 2026 GMT
  host: kadence.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: api.onkadence.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: api.us.onkadence.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kadence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kadence, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kadence
provider_slug: kadence
slug: kadence-domain-security
source_filename: kadence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kadence.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:06:02 2026 GMT\n  hsts: null\n- host: api.onkadence.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\n- host: api.us.onkadence.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kadence.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: onkadence.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/security/kadence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Workplace
- Hybrid Work
- Desk Booking
- Room Booking
- Space Management
- Visitor Management
- Workplace Analytics
- Facilities
- OAuth
---
