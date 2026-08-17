---
api_specs:
- filename: trade-desk-advertiser-api-openapi.yml
  format: yaml
  label: The Trade Desk Advertiser API
  slug: trade-desk-advertiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-advertiser-api-openapi.yml
- filename: trade-desk-deletionoptout-api-openapi.yml
  format: yaml
  label: The Trade Desk DeletionOptOut API
  slug: trade-desk-deletionoptout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-deletionoptout-api-openapi.yml
- filename: trade-desk-offlineconversion-api-openapi.yml
  format: yaml
  label: The Trade Desk OfflineConversion API
  slug: trade-desk-offlineconversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-offlineconversion-api-openapi.yml
- filename: trade-desk-thirdparty-api-openapi.yml
  format: yaml
  label: The Trade Desk ThirdParty API
  slug: trade-desk-thirdparty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-thirdparty-api-openapi.yml
- filename: trade-desk-ipaddress-api-openapi.yml
  format: yaml
  label: The Trade Desk IPAddress Data API
  slug: trade-desk-ipaddress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-ipaddress-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thetradedesk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adsrvr.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sincera.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uidapi.com
  spf: false
hosts:
- cert_expires: Oct 23 20:55:21 2026 GMT
  host: www.thetradedesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: partner.thetradedesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: api.thetradedesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: open.thetradedesk.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: auth.thetradedesk.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: usw-data.adsrvr.org
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: offlineattrib.adsrvr.org
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: insight.adsrvr.org
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 08:23:39 2026 GMT
  host: open.sincera.io
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: prod.uidapi.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trade Desk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Trade Desk, probed live across 10 host(s) and 4 registrable domain(s). 10 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Trade Desk
provider_slug: trade-desk
slug: trade-desk-domain-security
source_filename: trade-desk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thetradedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 20:55:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner.thetradedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: null\n- host: api.thetradedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: null\n- host: open.thetradedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n- host: auth.thetradedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n- host: usw-data.adsrvr.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n- host: offlineattrib.adsrvr.org\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n- host: insight.adsrvr.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n- host: open.sincera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 08:23:39 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: prod.uidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\ndomains:\n- domain: thetradedesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adsrvr.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sincera.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: uidapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\nnote: The mechanical probe\
  \ caps at three hosts and one registrable domain. The additional hosts and domains\n  below were probed by hand on 2026-08-13 with the same method, to cover the API, auth, data-ingest, OpenSincera\n  and UID2 operator surfaces. No HSTS on any host except www.thetradedesk.com; no CAA and no DNSSEC on\n  any Trade Desk domain. DMARC is p=reject across thetradedesk.com, adsrvr.org, sincera.io and uidapi.com,\n  with adsrvr.org and uidapi.com aggregate reports routing to secops@thetradedesk.com — which is a useful\n  ownership signal for those two non-thetradedesk.com domains.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/security/trade-desk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Programmatic Advertising
- Demand-Side Platform
- DSP
- AdTech
- Connected TV
- CTV
- Identity
- Unified ID 2.0
- UID2
- OpenPath
- Kokai
- Koa AI
- Galileo
- Sincera
- Open Internet
- Real-Time Bidding
- Open Measurement
---
