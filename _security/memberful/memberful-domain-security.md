---
api_specs:
- filename: memberful.postman_collection.json
  format: json
  label: Memberful Members API
  slug: memberful-members-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/memberful/refs/heads/main/collections/memberful.postman_collection.json
- filename: memberful.postman_collection.json
  format: json
  label: Memberful Subscriptions API
  slug: memberful-subscriptions-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/memberful/refs/heads/main/collections/memberful.postman_collection.json
- filename: memberful.postman_collection.json
  format: json
  label: Memberful Plans and Passes API
  slug: memberful-plans-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/memberful/refs/heads/main/collections/memberful.postman_collection.json
- filename: memberful.postman_collection.json
  format: json
  label: Memberful Orders API
  slug: memberful-orders-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/memberful/refs/heads/main/collections/memberful.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memberful.com
  spf: true
hosts:
- cert_expires: Aug 28 20:25:57 2026 GMT
  host: memberful.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 02:42:31 2026 GMT
  host: account.memberful.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memberful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memberful, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Memberful
provider_slug: memberful
slug: memberful-domain-security
source_filename: memberful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memberful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 20:25:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: account.memberful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:42:31 2026 GMT\n  hsts: null\ndomains:\n- domain: memberful.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memberful/refs/heads/main/security/memberful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Memberships
- Subscriptions
- Payments
- Creators
- GraphQL
- Patreon
---
