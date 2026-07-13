---
api_specs:
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Accounts API
  slug: badger-maps-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Locations API
  slug: badger-maps-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Check-Ins API
  slug: badger-maps-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Routes API
  slug: badger-maps-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Users API
  slug: badger-maps-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: badgermapping.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Mar 26 14:25:12 2027 GMT
  host: www.badgermapping.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: badgerupdatedapi.docs.apiary.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 03:46:46 2026 GMT
  host: badgerapis.badgermapping.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Badger Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Badger Maps, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Badger Maps
provider_slug: badger-maps
slug: badger-maps-domain-security
source_filename: badger-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.badgermapping.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 26 14:25:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: badgerupdatedapi.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: badgerapis.badgermapping.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 03:46:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: badgermapping.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/security/badger-maps-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Field Sales
- Route Planning
- Mapping
- CRM
- Sales Enablement
- Territory Management
---
