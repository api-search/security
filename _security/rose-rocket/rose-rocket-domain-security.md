---
api_specs:
- filename: rose-rocket-boards-api-openapi.yml
  format: yaml
  label: Rose Rocket Boards API
  slug: rose-rocket-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-boards-api-openapi.yml
- filename: rose-rocket-events-api-openapi.yml
  format: yaml
  label: Rose Rocket Events API
  slug: rose-rocket-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-events-api-openapi.yml
- filename: rose-rocket-object-records-api-openapi.yml
  format: yaml
  label: Rose Rocket Object Records API
  slug: rose-rocket-object-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-object-records-api-openapi.yml
- filename: rose-rocket-user-groups-api-openapi.yml
  format: yaml
  label: Rose Rocket User Groups API
  slug: rose-rocket-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-user-groups-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: roserocket.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Nov 24 12:25:58 2026 GMT
  host: www.roserocket.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: roserocket.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 12:25:58 2026 GMT
  host: network.roserocket.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rose Rocket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rose Rocket, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rose Rocket
provider_slug: rose-rocket
slug: rose-rocket-domain-security
source_filename: rose-rocket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roserocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 12:25:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: roserocket.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: network.roserocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 12:25:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: roserocket.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/security/rose-rocket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation
- Logistics
- freight
- trucking
- transportation-management-system
- Supply Chain
- dispatch
- Webhook
- Authentication
- canada
---
