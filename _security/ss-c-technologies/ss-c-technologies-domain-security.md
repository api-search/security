---
api_specs:
- filename: ss-c-technologies-marketdataservice-api-openapi.yml
  format: yaml
  label: SS&C Technologies Market Data Service API
  slug: ss-c-technologies-marketdataservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-marketdataservice-api-openapi.yml
- filename: ss-c-technologies-submitorderservice-api-openapi.yml
  format: yaml
  label: SS&C Technologies Submit Order Service API
  slug: ss-c-technologies-submitorderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-submitorderservice-api-openapi.yml
- filename: ss-c-technologies-userservices-api-openapi.yml
  format: yaml
  label: SS&C Technologies User Services API
  slug: ss-c-technologies-userservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-userservices-api-openapi.yml
- filename: ss-c-technologies-xapiserver-api-openapi.yml
  format: yaml
  label: SS&C Technologies XAPI Server API
  slug: ss-c-technologies-xapiserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-xapiserver-api-openapi.yml
- filename: ss-c-technologies-utility-services-api-openapi.yml
  format: yaml
  label: SS&C Technologies Utility Services API
  slug: ss-c-technologies-utility-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-utility-services-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ssctech.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: taltrade.com
  spf: false
hosts:
- cert_expires: Oct 28 21:34:31 2026 GMT
  host: www.ssctech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: emsuatxapi.taltrade.com
  https: false
  note: 'The probe tests port 443, which this host does not serve. The published Eze EMS xAPI REST endpoint is https://emsuatxapi.taltrade.com:9001 and a direct fetch of https://emsuatxapi.taltrade.com:9001/swagger/v1/swagger.json completed a TLS handshake and returned HTTP 200 on 2026-09-13, so `https: false` here means "nothing on 443", not "no TLS".'
- cert_expires: Nov  4 11:56:05 2026 GMT
  host: developer.ssctech.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ss C Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SS&C Technologies, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SS&C Technologies
provider_slug: ss-c-technologies
slug: ss-c-technologies-domain-security
source_filename: ss-c-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ssctech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 21:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: emsuatxapi.taltrade.com\n  https: false\n  note: >-\n    The probe tests port 443, which this host does not serve. The published Eze EMS xAPI REST\n    endpoint is https://emsuatxapi.taltrade.com:9001 and a direct fetch of\n    https://emsuatxapi.taltrade.com:9001/swagger/v1/swagger.json completed a TLS handshake and\n    returned HTTP 200 on 2026-09-13, so `https: false` here means \"nothing on 443\", not \"no TLS\".\n- host: developer.ssctech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:56:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ssctech.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  -\
  \ 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: taltrade.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/security/ss-c-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Investment Management
- Fund Administration
- Wealth Management
- Execution Management
- Order Management
- Market Data
- Trading
- gRPC
- Enterprise Software
---
