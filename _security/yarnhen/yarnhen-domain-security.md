---
api_specs:
- filename: yarnhen-accounts-api-openapi.yml
  format: yaml
  label: Yarnhen Accounts API
  slug: yarnhen-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-accounts-api-openapi.yml
- filename: yarnhen-discovery-api-openapi.yml
  format: yaml
  label: Yarnhen Discovery API
  slug: yarnhen-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-discovery-api-openapi.yml
- filename: yarnhen-posts-api-openapi.yml
  format: yaml
  label: Yarnhen Posts API
  slug: yarnhen-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-posts-api-openapi.yml
- filename: yarnhen-webhooks-api-openapi.yml
  format: yaml
  label: Yarnhen Webhooks API
  slug: yarnhen-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yarnhen.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yawplet.com
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: yarnhen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: yawplet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: hagglebee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Yarnhen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yarnhen, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yarnhen
provider_slug: yarnhen
slug: yarnhen-domain-security
source_filename: yarnhen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yarnhen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yawplet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hagglebee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yarnhen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: yawplet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/security/yarnhen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- MCP
- Publishing
- Stories
- Content Moderation
- Creative Commons
---
