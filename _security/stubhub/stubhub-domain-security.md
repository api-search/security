---
api_specs:
- filename: stubhub-addressess-api-openapi.yml
  format: yaml
  label: StubHub Addressess API
  slug: stubhub-addressess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-addressess-api-openapi.yml
- filename: stubhub-categories-api-openapi.yml
  format: yaml
  label: StubHub Categories API
  slug: stubhub-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-categories-api-openapi.yml
- filename: stubhub-e-tickets-api-openapi.yml
  format: yaml
  label: StubHub E-Tickets API
  slug: stubhub-e-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-e-tickets-api-openapi.yml
- filename: stubhub-events-api-openapi.yml
  format: yaml
  label: StubHub Events API
  slug: stubhub-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-events-api-openapi.yml
- filename: stubhub-listingconstraints-api-openapi.yml
  format: yaml
  label: StubHub ListingConstraints API
  slug: stubhub-listingconstraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-listingconstraints-api-openapi.yml
- filename: stubhub-paymentmethods-api-openapi.yml
  format: yaml
  label: StubHub PaymentMethods API
  slug: stubhub-paymentmethods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-paymentmethods-api-openapi.yml
- filename: stubhub-payments-api-openapi.yml
  format: yaml
  label: StubHub Payments API
  slug: stubhub-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-payments-api-openapi.yml
- filename: stubhub-sales-api-openapi.yml
  format: yaml
  label: StubHub Sales API
  slug: stubhub-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-sales-api-openapi.yml
- filename: stubhub-sellerevents-api-openapi.yml
  format: yaml
  label: StubHub SellerEvents API
  slug: stubhub-sellerevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-sellerevents-api-openapi.yml
- filename: stubhub-sellerlistings-api-openapi.yml
  format: yaml
  label: StubHub SellerListings API
  slug: stubhub-sellerlistings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-sellerlistings-api-openapi.yml
- filename: stubhub-shipments-api-openapi.yml
  format: yaml
  label: StubHub Shipments API
  slug: stubhub-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-shipments-api-openapi.yml
- filename: stubhub-ticketholders-api-openapi.yml
  format: yaml
  label: StubHub TicketHolders API
  slug: stubhub-ticketholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-ticketholders-api-openapi.yml
- filename: stubhub-user-api-openapi.yml
  format: yaml
  label: StubHub User API
  slug: stubhub-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-user-api-openapi.yml
- filename: stubhub-venues-api-openapi.yml
  format: yaml
  label: StubHub Venues API
  slug: stubhub-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-venues-api-openapi.yml
- filename: stubhub-webhooks-api-openapi.yml
  format: yaml
  label: StubHub Webhooks API
  slug: stubhub-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stubhub.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: stubhub.net
  spf: false
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.stubhub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.stubhub.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: sandbox.api.stubhub.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stubhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StubHub, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: StubHub
provider_slug: stubhub
slug: stubhub-domain-security
source_filename: stubhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stubhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stubhub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox.api.stubhub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: stubhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stubhub.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/security/stubhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplaces
- Tickets
- Event
- Ticketing
- Live Events
- Secondary Market
- E-Commerce
- Sports
- Concerts
---
