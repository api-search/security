---
api_specs:
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Bookings API
  slug: ownerrez-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Properties API
  slug: ownerrez-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Listings API
  slug: ownerrez-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Guests API
  slug: ownerrez-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Inquiries API
  slug: ownerrez-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Quotes API
  slug: ownerrez-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Reviews API
  slug: ownerrez-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Messages API
  slug: ownerrez-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Custom Fields and Tags API
  slug: ownerrez-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Payments and Financials API
  slug: ownerrez-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Webhook Subscriptions API
  slug: ownerrez-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ownerrez.com
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.ownerrez.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: api.ownerrez.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ownerrez Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OwnerRez, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OwnerRez
provider_slug: ownerrez
slug: ownerrez-domain-security
source_filename: ownerrez-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ownerrez.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.ownerrez.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ownerrez.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/security/ownerrez-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Vacation Rental
- Short-Term Rental
- Property Management
- Hospitality
- Bookings
- Channel Manager
---
