---
api_specs:
- filename: talkable-v2-openapi-original.yml
  format: yaml
  label: Talkable API v2
  slug: talkable-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/openapi/talkable-v2-openapi-original.yml
- filename: talkable-webhooks-openapi-original.yml
  format: yaml
  label: Talkable Webhooks
  slug: talkable-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/openapi/talkable-webhooks-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: talkable.com
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: talkable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: docs.talkable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: www.talkable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talkable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talkable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Talkable
provider_slug: talkable
slug: talkable-domain-security
source_filename: talkable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talkable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.talkable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: www.talkable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: talkable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/security/talkable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Referral Marketing
- Loyalty
- Marketing
- E-commerce
- Advocacy
- Rewards
- Customer Acquisition
- Webhooks
- MCP
---
