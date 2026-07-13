---
api_specs:
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Properties API
  slug: hospitable-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Listings API
  slug: hospitable-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Reservations API
  slug: hospitable-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Messages API
  slug: hospitable-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Calendar API
  slug: hospitable-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Reviews API
  slug: hospitable-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hospitable.com
  spf: true
hosts:
- cert_expires: Sep 10 00:38:59 2026 GMT
  host: hospitable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 09:46:45 2026 GMT
  host: developer.hospitable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 08:11:58 2026 GMT
  host: public.api.hospitable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hospitable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hospitable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hospitable
provider_slug: hospitable
slug: hospitable-domain-security
source_filename: hospitable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hospitable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 00:38:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hospitable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:46:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.api.hospitable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:11:58 2026 GMT\n  hsts: null\ndomains:\n- domain: hospitable.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/security/hospitable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Vacation Rental
- Short-Term Rental
- Property Management
- Airbnb
- Hospitality
- Automation
---
