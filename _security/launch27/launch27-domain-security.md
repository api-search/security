---
api_specs:
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Authentication API
  slug: launch27-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Account Settings API
  slug: launch27-account-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Booking Helpers API
  slug: launch27-booking-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Booking Policies API
  slug: launch27-booking-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Guest Booking API
  slug: launch27-guest-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Customer Bookings API
  slug: launch27-customer-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: launch27.com
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:root@bitbucket.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitbucket.org
  spf: true
hosts:
- cert_expires: Aug  8 19:24:11 2026 GMT
  host: www.launch27.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: bitbucket.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Launch27 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Launch27, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Launch27
provider_slug: launch27
slug: launch27-domain-security
source_filename: launch27-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.launch27.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 19:24:11 2026 GMT\n  hsts: false\n- host: bitbucket.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: launch27.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bitbucket.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:root@bitbucket.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/security/launch27-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- Home Services
- Cleaning Services
- Booking
- Scheduling
- Fullsteam
- Vonigo
---
