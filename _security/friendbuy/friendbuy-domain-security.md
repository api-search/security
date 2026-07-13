---
api_specs:
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Customers API
  slug: friendbuy-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Referrals API
  slug: friendbuy-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Events API
  slug: friendbuy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Analytics API
  slug: friendbuy-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Rewards & Loyalty API
  slug: friendbuy-rewards-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: friendbuy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fbot.me
  spf: false
hosts:
- cert_expires: Aug  4 23:12:28 2026 GMT
  host: friendbuy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: developers.friendbuy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: mapi.fbot.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Friendbuy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Friendbuy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Friendbuy
provider_slug: friendbuy
slug: friendbuy-domain-security
source_filename: friendbuy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: friendbuy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 23:12:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.friendbuy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\n- host: mapi.fbot.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: friendbuy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fbot.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/security/friendbuy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Referral Marketing
- Loyalty
- Rewards
- Ecommerce
- Marketing
- Advocacy
---
