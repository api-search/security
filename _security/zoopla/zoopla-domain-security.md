---
api_specs:
- filename: zoopla-leads-api-openapi.json
  format: json
  label: Zoopla Leads API
  slug: zoopla-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-leads-api-openapi.json
- filename: zoopla-premium-listing-activations-openapi.json
  format: json
  label: Zoopla Premium Listing Activations API
  slug: zoopla-premium-listing-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-premium-listing-activations-openapi.json
- filename: zoopla-weekly-featured-property-activations-openapi.json
  format: json
  label: Zoopla Weekly Featured Property (WFP) Activations API
  slug: zoopla-weekly-featured-property-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-weekly-featured-property-activations-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoopla.co.uk
  spf: true
hosts:
- cert_expires: Sep 12 23:27:27 2026 GMT
  host: www.zoopla.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 03:21:18 2026 GMT
  host: developers.zoopla.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: services.zoopla.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoopla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoopla, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoopla
provider_slug: zoopla
slug: zoopla-domain-security
source_filename: zoopla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoopla.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:27:27 2026 GMT\n  hsts: null\n- host: developers.zoopla.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:21:18 2026 GMT\n  hsts: false\n- host: services.zoopla.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zoopla.co.uk\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/security/zoopla-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Property Portal
- PropTech
- Rentals
- Estate Agents
- Leads
- CRM Integration
---
