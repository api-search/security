---
api_specs:
- filename: liqaa-io-conversations-api-openapi.yml
  format: yaml
  label: LIQAA Conversations API
  slug: liqaa-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liqaa-io/openapi/liqaa-io-conversations-api-openapi.yml
- filename: liqaa-io-tokens-api-openapi.yml
  format: yaml
  label: LIQAA Tokens API
  slug: liqaa-io-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liqaa-io/openapi/liqaa-io-tokens-api-openapi.yml
- filename: liqaa-io-webhooks-api-openapi.yml
  format: yaml
  label: LIQAA Webhooks API
  slug: liqaa-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liqaa-io/openapi/liqaa-io-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:DIRECTION@takawen.dz"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: liqaa.io
  spf: true
hosts:
- host: liqaa.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LIQAA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LIQAA, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LIQAA
provider_slug: liqaa-io
slug: liqaa-io-domain-security
source_filename: liqaa-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liqaa.io\n  https: false\ndomains:\n- domain: liqaa.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:DIRECTION@takawen.dz\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/liqaa-io/security/liqaa-io-domain-security.yml
summary_line: DMARC
tags:
- Video
- Messaging
- SDK
- Real-Time
- Algeria
- Company
---
