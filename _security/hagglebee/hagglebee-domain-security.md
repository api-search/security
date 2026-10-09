---
api_specs:
- filename: hagglebee-accounts-api-openapi.yml
  format: yaml
  label: Hagglebee Accounts API
  slug: hagglebee-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/openapi/hagglebee-accounts-api-openapi.yml
- filename: hagglebee-discovery-api-openapi.yml
  format: yaml
  label: Hagglebee Discovery API
  slug: hagglebee-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/openapi/hagglebee-discovery-api-openapi.yml
- filename: hagglebee-posts-api-openapi.yml
  format: yaml
  label: Hagglebee Posts API
  slug: hagglebee-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/openapi/hagglebee-posts-api-openapi.yml
- filename: hagglebee-webhooks-api-openapi.yml
  format: yaml
  label: Hagglebee Webhooks API
  slug: hagglebee-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/openapi/hagglebee-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hagglebee.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yawplet.com
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: hagglebee.com
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
name: Hagglebee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hagglebee, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hagglebee
provider_slug: hagglebee
slug: hagglebee-domain-security
source_filename: hagglebee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hagglebee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yawplet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yarnhen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hagglebee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: yawplet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/security/hagglebee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- MCP
- Classifieds
- Marketplace
- Content Moderation
- Publishing
---
