---
api_specs:
- filename: rea-group-oauth-openapi.yml
  format: yaml
  label: PropTrack OAuth 2.0 Token API
  slug: proptrack-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-oauth-openapi.yml
- filename: rea-group-address-openapi.yml
  format: yaml
  label: PropTrack Address API
  slug: proptrack-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-address-openapi.yml
- filename: rea-group-properties-openapi.yml
  format: yaml
  label: PropTrack Properties API
  slug: proptrack-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-properties-openapi.yml
- filename: rea-group-listings-openapi.yml
  format: yaml
  label: PropTrack Listings API
  slug: proptrack-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-listings-openapi.yml
- filename: rea-group-transactions-openapi.yml
  format: yaml
  label: PropTrack Transactions API
  slug: proptrack-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-transactions-openapi.yml
- filename: rea-group-market-openapi.yml
  format: yaml
  label: PropTrack Market API
  slug: proptrack-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-market-openapi.yml
- filename: rea-group-reports-openapi.yml
  format: yaml
  label: PropTrack Reports API
  slug: proptrack-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-reports-openapi.yml
- filename: rea-group-disclaimers-openapi.yml
  format: yaml
  label: PropTrack Disclaimers API
  slug: proptrack-disclaimers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-disclaimers-openapi.yml
- filename: rea-group-coming-soon-openapi.yml
  format: yaml
  label: PropTrack Upcoming APIs (Schools)
  slug: proptrack-upcoming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-coming-soon-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@rea-group.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rea-group.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:pt-systems-support@rea-group.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: proptrack.com.au
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.rea-group.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:33:34 2026 GMT
  host: developer.proptrack.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:37:58 2026 GMT
  host: data.proptrack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rea Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REA Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: REA Group
provider_slug: rea-group
slug: rea-group-domain-security
source_filename: rea-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rea-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.proptrack.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:33:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.proptrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:37:58 2026 GMT\n  hsts: null\ndomains:\n- domain: rea-group.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@rea-group.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: proptrack.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:pt-systems-support@rea-group.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/security/rea-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Property Data
- Valuations
- AVM
- Market Insights
- Listings
- Transaction
- Address Matching
- REAXML
- Partner Portal
- PropTech
- Australia
---
