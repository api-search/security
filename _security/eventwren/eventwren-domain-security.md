---
api_specs:
- filename: eventwren-accounts-api-openapi.yml
  format: yaml
  label: Eventwren Accounts API
  slug: eventwren-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-accounts-api-openapi.yml
- filename: eventwren-discovery-api-openapi.yml
  format: yaml
  label: Eventwren Discovery API
  slug: eventwren-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-discovery-api-openapi.yml
- filename: eventwren-posts-api-openapi.yml
  format: yaml
  label: Eventwren Posts API
  slug: eventwren-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-posts-api-openapi.yml
- filename: eventwren-webhooks-api-openapi.yml
  format: yaml
  label: Eventwren Webhooks API
  slug: eventwren-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eventwren.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yawplet.com
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: eventwren.com
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
  host: yarnhen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Eventwren Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eventwren, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eventwren
provider_slug: eventwren
slug: eventwren-domain-security
source_filename: eventwren-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventwren.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yawplet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yarnhen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eventwren.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: yawplet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/security/eventwren-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- MCP
- Event
- Calendar
- Content Moderation
- Publishing
---
