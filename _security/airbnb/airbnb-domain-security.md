---
api_specs:
- filename: airbnb-webhooks-asyncapi.yml
  format: yaml
  label: Airbnb Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/asyncapi/airbnb-webhooks-asyncapi.yml
- filename: airbnb-bookings-api-openapi.yml
  format: yaml
  label: airbnb Bookings API
  slug: airbnb-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-bookings-api-openapi.yml
- filename: airbnb-calendar-api-openapi.yml
  format: yaml
  label: airbnb Calendar API
  slug: airbnb-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-calendar-api-openapi.yml
- filename: airbnb-experience-messages-api-openapi.yml
  format: yaml
  label: airbnb Experience Messages API
  slug: airbnb-experience-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-experience-messages-api-openapi.yml
- filename: airbnb-experiences-api-openapi.yml
  format: yaml
  label: airbnb Experiences API
  slug: airbnb-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-experiences-api-openapi.yml
- filename: airbnb-listings-api-openapi.yml
  format: yaml
  label: airbnb Listings API
  slug: airbnb-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-listings-api-openapi.yml
- filename: airbnb-messages-api-openapi.yml
  format: yaml
  label: airbnb Messages API
  slug: airbnb-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-messages-api-openapi.yml
- filename: airbnb-photos-api-openapi.yml
  format: yaml
  label: airbnb Photos API
  slug: airbnb-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-photos-api-openapi.yml
- filename: airbnb-reservations-api-openapi.yml
  format: yaml
  label: airbnb Reservations API
  slug: airbnb-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-reservations-api-openapi.yml
- filename: airbnb-reviews-api-openapi.yml
  format: yaml
  label: airbnb Reviews API
  slug: airbnb-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-reviews-api-openapi.yml
- filename: airbnb-schedules-api-openapi.yml
  format: yaml
  label: airbnb Schedules API
  slug: airbnb-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-schedules-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:caa-alerts@airbnb.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airbnb.com
  spf: true
- caa:
  - 0 iodef "mailto:caa-alerts@airbnb.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: withairbnb.com
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: www.airbnb.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:34:56 2026 GMT
  host: developer.withairbnb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: api.airbnb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airbnb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for airbnb, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: airbnb
provider_slug: airbnb
slug: airbnb-domain-security
source_filename: airbnb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airbnb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: developer.withairbnb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:34:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.airbnb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: airbnb.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:caa-alerts@airbnb.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: withairbnb.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa-alerts@airbnb.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/security/airbnb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
