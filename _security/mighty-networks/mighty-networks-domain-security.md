---
api_specs:
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Members API
  slug: mighty-networks-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Spaces API
  slug: mighty-networks-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Posts API
  slug: mighty-networks-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Comments and Reactions API
  slug: mighty-networks-comments-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Events and RSVPs API
  slug: mighty-networks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Courses API
  slug: mighty-networks-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Plans and Subscriptions API
  slug: mighty-networks-plans-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Invites API
  slug: mighty-networks-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Badges and Tags API
  slug: mighty-networks-badges-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Custom Fields API
  slug: mighty-networks-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Polls and Questions API
  slug: mighty-networks-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Network and Collections API
  slug: mighty-networks-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Webhooks
  slug: mighty-networks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mightynetworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mn.co
  spf: true
hosts:
- cert_expires: Aug 17 02:24:29 2026 GMT
  host: www.mightynetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 21:15:18 2026 GMT
  host: docs.mightynetworks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:43:14 2026 GMT
  host: api.mn.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mighty Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mighty Networks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mighty Networks
provider_slug: mighty-networks
slug: mighty-networks-domain-security
source_filename: mighty-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mightynetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 02:24:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mightynetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:15:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mn.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:43:14 2026 GMT\n  hsts: null\ndomains:\n- domain: mightynetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mn.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/security/mighty-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Community
- Courses
- Membership
- Creator Economy
- Events
- Subscriptions
---
