---
api_specs:
- filename: api_v2.json
  format: json
  label: Instantly Campaigns API
  slug: campaigns-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Leads API
  slug: leads-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Accounts API
  slug: accounts-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Email Verification API
  slug: email-verification-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Inbox Placement Test API
  slug: inbox-placement-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly API Keys API
  slug: api-keys-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Workspaces API
  slug: workspaces-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: instantly.ai
  spf: true
hosts:
- cert_expires: Aug 12 18:35:30 2026 GMT
  host: instantly.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 05:39:37 2026 GMT
  host: developer.instantly.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 16:03:27 2026 GMT
  host: api.instantly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instantly Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instantly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Instantly
provider_slug: instantly-ai
slug: instantly-ai-domain-security
source_filename: instantly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instantly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 18:35:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.instantly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:39:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.instantly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:03:27 2026 GMT\n  hsts: false\ndomains:\n- domain: instantly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instantly-ai/refs/heads/main/security/instantly-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cold Email
- Outbound
- Sales
- Deliverability
- Lead Database
- Email Verification
- Webhooks
---
