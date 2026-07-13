---
api_specs:
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Customers API
  slug: vimeo-ott-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Products API
  slug: vimeo-ott-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Videos API
  slug: vimeo-ott-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Collections API
  slug: vimeo-ott-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Authorizations API
  slug: vimeo-ott-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Analytics API
  slug: vimeo-ott-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vimeo.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vhx.tv
  spf: true
hosts:
- cert_expires: Oct  4 13:14:00 2026 GMT
  host: vimeo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 08:31:42 2026 GMT
  host: dev.vhx.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 16:57:19 2026 GMT
  host: api.vhx.tv
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vimeo Ott Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vimeo OTT, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vimeo OTT
provider_slug: vimeo-ott
slug: vimeo-ott-domain-security
source_filename: vimeo-ott-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vimeo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:14:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.vhx.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 08:31:42 2026 GMT\n  hsts: false\n- host: api.vhx.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:57:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vimeo.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vhx.tv\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\
  \n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/security/vimeo-ott-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- OTT
- Video
- SVOD
- Streaming
- Media
- Subscriptions
- VHX
---
