---
api_specs:
- filename: yawplet-accounts-api-openapi.yml
  format: yaml
  label: Yawplet Accounts API
  slug: yawplet-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/openapi/yawplet-accounts-api-openapi.yml
- filename: yawplet-discovery-api-openapi.yml
  format: yaml
  label: Yawplet Discovery API
  slug: yawplet-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/openapi/yawplet-discovery-api-openapi.yml
- filename: yawplet-posts-api-openapi.yml
  format: yaml
  label: Yawplet Posts API
  slug: yawplet-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/openapi/yawplet-posts-api-openapi.yml
- filename: yawplet-webhooks-api-openapi.yml
  format: yaml
  label: Yawplet Webhooks API
  slug: yawplet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/openapi/yawplet-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yawplet.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yarnhen.com
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: yawplet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: yarnhen.com
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
name: Yawplet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yawplet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yawplet
provider_slug: yawplet
slug: yawplet-domain-security
source_filename: yawplet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yawplet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yarnhen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hagglebee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yawplet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: yarnhen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/security/yawplet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- MCP
- Social Media
- Messaging
- Content Moderation
- Publishing
---
