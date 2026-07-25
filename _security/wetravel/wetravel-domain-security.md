---
api_specs:
- filename: wetravel-access-token-api-openapi.yml
  format: yaml
  label: WeTravel Access token API
  slug: wetravel-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-access-token-api-openapi.yml
- filename: wetravel-add-ons-api-openapi.yml
  format: yaml
  label: WeTravel Add-ons API
  slug: wetravel-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-add-ons-api-openapi.yml
- filename: wetravel-discounts-api-openapi.yml
  format: yaml
  label: WeTravel Discounts API
  slug: wetravel-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-discounts-api-openapi.yml
- filename: wetravel-images-api-openapi.yml
  format: yaml
  label: WeTravel Images API
  slug: wetravel-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-images-api-openapi.yml
- filename: wetravel-included-items-api-openapi.yml
  format: yaml
  label: WeTravel Included items API
  slug: wetravel-included-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-included-items-api-openapi.yml
- filename: wetravel-leads-api-openapi.yml
  format: yaml
  label: WeTravel Leads API
  slug: wetravel-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-leads-api-openapi.yml
- filename: wetravel-not-included-items-api-openapi.yml
  format: yaml
  label: WeTravel Not Included items API
  slug: wetravel-not-included-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-not-included-items-api-openapi.yml
- filename: wetravel-orders-api-openapi.yml
  format: yaml
  label: WeTravel Orders API
  slug: wetravel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-orders-api-openapi.yml
- filename: wetravel-packages-api-openapi.yml
  format: yaml
  label: WeTravel Packages API
  slug: wetravel-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-packages-api-openapi.yml
- filename: wetravel-paragraphs-api-openapi.yml
  format: yaml
  label: WeTravel Paragraphs API
  slug: wetravel-paragraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-paragraphs-api-openapi.yml
- filename: wetravel-participant-information-api-openapi.yml
  format: yaml
  label: WeTravel Participant Information API
  slug: wetravel-participant-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-participant-information-api-openapi.yml
- filename: wetravel-payment-links-api-openapi.yml
  format: yaml
  label: WeTravel Payment Links API
  slug: wetravel-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-payment-links-api-openapi.yml
- filename: wetravel-payment-plans-api-openapi.yml
  format: yaml
  label: WeTravel Payment Plans API
  slug: wetravel-payment-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-payment-plans-api-openapi.yml
- filename: wetravel-suppliers-api-openapi.yml
  format: yaml
  label: WeTravel Suppliers API
  slug: wetravel-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-suppliers-api-openapi.yml
- filename: wetravel-transactions-api-openapi.yml
  format: yaml
  label: WeTravel Transactions API
  slug: wetravel-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-transactions-api-openapi.yml
- filename: wetravel-trip-overview-api-openapi.yml
  format: yaml
  label: WeTravel Trip Overview API
  slug: wetravel-trip-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-trip-overview-api-openapi.yml
- filename: wetravel-trips-api-openapi.yml
  format: yaml
  label: WeTravel Trips API
  slug: wetravel-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-trips-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wetravel.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wetravel.to
  spf: true
hosts:
- cert_expires: Sep 10 14:13:36 2026 GMT
  host: www.wetravel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:02:04 2026 GMT
  host: api.wetravel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 19:09:44 2026 GMT
  host: api.demo.wetravel.to
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wetravel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeTravel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: WeTravel
provider_slug: wetravel
slug: wetravel-domain-security
source_filename: wetravel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wetravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:13:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wetravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:02:04 2026 GMT\n  hsts: null\n- host: api.demo.wetravel.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 19:09:44 2026 GMT\n  hsts: null\ndomains:\n- domain: wetravel.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wetravel.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/security/wetravel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- Travel
- Booking
- Payments
- Trip Management
- Tour Operators
- Travel Technology
---
