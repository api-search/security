---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Xoxoday Plum Rewards API
  slug: plum-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoxoday/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: xoxoday.com
  spf: true
hosts:
- cert_expires: Sep  8 09:51:20 2026 GMT
  host: www.xoxoday.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 21:42:53 2026 GMT
  host: developers.xoxoday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 06:44:44 2026 GMT
  host: accounts.xoxoday.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xoxoday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xoxoday, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Xoxoday
provider_slug: xoxoday
slug: xoxoday-domain-security
source_filename: xoxoday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xoxoday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:51:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.xoxoday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 21:42:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: accounts.xoxoday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:44:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: xoxoday.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xoxoday/refs/heads/main/security/xoxoday-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Rewards
- Employee Engagement
- Gift Cards
- Incentives
- Loyalty
- Recognition
- Digital Rewards
- Points Programs
- Redemption
- Fintech
---
