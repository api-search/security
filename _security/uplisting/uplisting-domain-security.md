---
api_specs:
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Bookings API
  slug: uplisting-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Properties API
  slug: uplisting-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Availability API
  slug: uplisting-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Calendar API
  slug: uplisting-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Rates API
  slug: uplisting-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Guests API
  slug: uplisting-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Messages API
  slug: uplisting-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Webhooks API
  slug: uplisting-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "zerossl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uplisting.io
  spf: true
hosts:
- cert_expires: Sep 27 09:43:38 2026 GMT
  host: www.uplisting.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 14:01:48 2026 GMT
  host: support.uplisting.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 01:06:43 2026 GMT
  host: connect.uplisting.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uplisting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uplisting, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uplisting
provider_slug: uplisting
slug: uplisting-domain-security
source_filename: uplisting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uplisting.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:43:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.uplisting.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:01:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: connect.uplisting.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uplisting.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"zerossl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/security/uplisting-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vacation Rental
- Short-Term Rental
- Channel Manager
- Property Management
- Bookings
- Hospitality
---
