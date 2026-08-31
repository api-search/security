---
api_specs:
- filename: memberpress-authentication-api-openapi.yml
  format: yaml
  label: MemberPress Authentication API
  slug: memberpress-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-authentication-api-openapi.yml
- filename: memberpress-coupons-api-openapi.yml
  format: yaml
  label: MemberPress Coupons API
  slug: memberpress-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-coupons-api-openapi.yml
- filename: memberpress-events-api-openapi.yml
  format: yaml
  label: MemberPress Events API
  slug: memberpress-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-events-api-openapi.yml
- filename: memberpress-groups-api-openapi.yml
  format: yaml
  label: MemberPress Groups API
  slug: memberpress-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-groups-api-openapi.yml
- filename: memberpress-members-api-openapi.yml
  format: yaml
  label: MemberPress Members API
  slug: memberpress-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-members-api-openapi.yml
- filename: memberpress-memberships-api-openapi.yml
  format: yaml
  label: MemberPress Memberships API
  slug: memberpress-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-memberships-api-openapi.yml
- filename: memberpress-reminders-api-openapi.yml
  format: yaml
  label: MemberPress Reminders API
  slug: memberpress-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-reminders-api-openapi.yml
- filename: memberpress-rules-api-openapi.yml
  format: yaml
  label: MemberPress Rules API
  slug: memberpress-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-rules-api-openapi.yml
- filename: memberpress-subscriptions-api-openapi.yml
  format: yaml
  label: MemberPress Subscriptions API
  slug: memberpress-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-subscriptions-api-openapi.yml
- filename: memberpress-transactions-api-openapi.yml
  format: yaml
  label: MemberPress Transactions API
  slug: memberpress-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-transactions-api-openapi.yml
- filename: memberpress-webhooks-api-openapi.yml
  format: yaml
  label: MemberPress Webhooks API
  slug: memberpress-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: memberpress.com
  spf: true
hosts:
- cert_expires: Oct  3 16:59:27 2026 GMT
  host: memberpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memberpress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MemberPress, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MemberPress
provider_slug: memberpress
slug: memberpress-domain-security
source_filename: memberpress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memberpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:59:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: memberpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/security/memberpress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Membership
- Subscription
- WordPress
- Payments
- E-Commerce
- Courses
- Content Management
- Webhook
- MCP
---
