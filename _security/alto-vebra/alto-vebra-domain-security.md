---
api_specs:
- filename: alto-api-openapi.json
  format: json
  label: Alto API
  slug: alto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/alto-api-openapi.json
- filename: zoopla-leads-api-openapi.json
  format: json
  label: Zoopla Leads API
  slug: zoopla-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-leads-api-openapi.json
- filename: zoopla-premium-listing-activations-openapi.json
  format: json
  label: Zoopla Premium Listing Activations API
  slug: zoopla-premium-listing-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-premium-listing-activations-openapi.json
- filename: zoopla-weekly-featured-property-openapi.json
  format: json
  label: Zoopla Weekly Featured Property (WFP) Activations API
  slug: zoopla-weekly-featured-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-weekly-featured-property-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: altosoftware.co.uk
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: vebraalto.com
  spf: false
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoopla.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoopladev.co.uk
  spf: false
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.alto.zoopla.co.uk
  hsts: false
  https: true
  role: Alto API production (OpenAPI servers[])
  tls_version: TLSv1.2
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.alto.zoopladev.co.uk
  hsts: false
  https: true
  role: Alto API sandbox (OpenAPI servers[], documented token endpoint)
  tls_version: TLSv1.2
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: services.zoopla.co.uk
  hsts: false
  https: true
  role: Zoopla product API host
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: services-auth.services.zoopla.co.uk
  hsts: false
  https: true
  role: Zoopla OAuth2 authorization server
  tls_version: TLSv1.3
- host: id.vebraalto.com
  hsts: false
  https: true
  role: Alto Connect identity provider (Auth0)
  tls_version: TLSv1.3
- cert_expires: Sep 12 19:28:33 2026 GMT
  host: www.altosoftware.co.uk
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: connect.vebraalto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: developers.vebraalto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alto Vebra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alto (Vebra / Zoopla), probed live across 8 host(s) and 4 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alto (Vebra / Zoopla)
provider_slug: alto-vebra
slug: alto-vebra-domain-security
source_filename: alto-vebra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The website/portal hosts were probed mechanically by 0-working/probe-domain-security.py; the\n  four API/auth hosts and the two Zoopla domains below were probed by hand in the same round\n  because they are declared only in OpenAPI servers[] and docs prose. Finding of record: not one\n  API host in this estate sets HSTS, and both Alto API hosts still negotiate TLSv1.2 while every\n  Zoopla host negotiates TLSv1.3.\nhosts:\n- host: api.alto.zoopla.co.uk\n  role: Alto API production (OpenAPI servers[])\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: false\n- host: api.alto.zoopladev.co.uk\n  role: Alto API sandbox (OpenAPI servers[], documented token endpoint)\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\n- host: services.zoopla.co.uk\n  role: Zoopla product API host\n  https:\
  \ true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\n- host: services-auth.services.zoopla.co.uk\n  role: Zoopla OAuth2 authorization server\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: id.vebraalto.com\n  role: Alto Connect identity provider (Auth0)\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n- host: www.altosoftware.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:28:33 2026 GMT\n  hsts: true\n- host: connect.vebraalto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: developers.vebraalto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: altosoftware.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vebraalto.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue\
  \ \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n- domain: zoopla.co.uk\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zoopladev.co.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/security/alto-vebra-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Listings
- CRM
- Property Management
- Rentals
- Conveyancing
- Estate Agency
- Tenancy
- Webhook
- Event
- Lettings
- Sales Progression
- Property Data
- Real Estate Software
---
