---
api_specs:
- filename: bidprowl-com-comps-api-openapi.yml
  format: yaml
  label: BidProwl Comps API
  slug: bidprowl-com-comps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-comps-api-openapi.yml
- filename: bidprowl-com-export-api-openapi.yml
  format: yaml
  label: BidProwl Export API
  slug: bidprowl-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-export-api-openapi.yml
- filename: bidprowl-com-flip-score-api-openapi.yml
  format: yaml
  label: BidProwl Flip Score API
  slug: bidprowl-com-flip-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-flip-score-api-openapi.yml
- filename: bidprowl-com-listings-api-openapi.yml
  format: yaml
  label: BidProwl Listings API
  slug: bidprowl-com-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-listings-api-openapi.yml
- filename: bidprowl-com-sold-api-openapi.yml
  format: yaml
  label: BidProwl Sold API
  slug: bidprowl-com-sold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-sold-api-openapi.yml
- filename: bidprowl-com-sources-api-openapi.yml
  format: yaml
  label: BidProwl Sources API
  slug: bidprowl-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-sources-api-openapi.yml
- filename: bidprowl-com-usage-api-openapi.yml
  format: yaml
  label: BidProwl Usage API
  slug: bidprowl-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-usage-api-openapi.yml
- filename: bidprowl-com-webhooks-api-openapi.yml
  format: yaml
  label: BidProwl Webhooks API
  slug: bidprowl-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bidprowl.com
  spf: true
hosts:
- cert_expires: Jan  1 18:02:52 2027 GMT
  host: bidprowl.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BidProwl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BidProwl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BidProwl
provider_slug: bidprowl-com
slug: bidprowl-com-domain-security
source_filename: bidprowl-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bidprowl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 18:02:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bidprowl.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bidprowl-com/security/bidprowl-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Auctions
- Marketplace
- Data
- Search
---
