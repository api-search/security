---
api_specs:
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Route Planning API
  slug: chargetrip-route-planning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Stations API
  slug: chargetrip-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Car Database API
  slug: chargetrip-car-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Isolines / Reachability API
  slug: chargetrip-isolines-reachability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Operators API
  slug: chargetrip-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chargetrip.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: chargetrip.io
  spf: false
hosts:
- cert_expires: Oct  4 04:46:13 2026 GMT
  host: www.chargetrip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: developers.chargetrip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.chargetrip.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chargetrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chargetrip, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Chargetrip
provider_slug: chargetrip
slug: chargetrip-domain-security
source_filename: chargetrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chargetrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:46:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.chargetrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.chargetrip.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chargetrip.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: chargetrip.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/security/chargetrip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- EV
- Routing
- Charging Stations
- GraphQL
- Mobility
---
