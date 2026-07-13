---
api_specs:
- filename: thanx-consumer-api-openapi.yml
  format: yaml
  label: Thanx Consumer API
  slug: consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-consumer-api-openapi.yml
- filename: thanx-partner-api-openapi.yml
  format: yaml
  label: Thanx Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-partner-api-openapi.yml
- filename: thanx-loyalty-api-openapi.yml
  format: yaml
  label: Thanx Loyalty API
  slug: loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-loyalty-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thanx.com
  spf: true
hosts:
- cert_expires: Aug 27 09:26:25 2026 GMT
  host: www.thanx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 05:31:22 2026 GMT
  host: docs.thanx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 04:16:41 2026 GMT
  host: api.thanx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thanx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thanx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thanx
provider_slug: thanx
slug: thanx-domain-security
source_filename: thanx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thanx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:26:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.thanx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 05:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.thanx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:16:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thanx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/security/thanx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Loyalty
- Guest Engagement
- Marketing
- CRM
- Online Ordering
- Webhooks
- Points
- Rewards
- Campaigns
---
