---
api_specs:
- filename: xproapi-default-api-openapi.yml
  format: yaml
  label: Xproapi Default API
  slug: xproapi-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-default-api-openapi.yml
- filename: xproapi-follow-followings-api-openapi.yml
  format: yaml
  label: Xproapi Follow, Followings API
  slug: xproapi-follow-followings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-follow-followings-api-openapi.yml
- filename: xproapi-tweet-activity-api-openapi.yml
  format: yaml
  label: Xproapi Tweet Activity API
  slug: xproapi-tweet-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-tweet-activity-api-openapi.yml
- filename: xproapi-tweets-api-openapi.yml
  format: yaml
  label: Xproapi Tweets API
  slug: xproapi-tweets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-tweets-api-openapi.yml
- filename: xproapi-users-api-openapi.yml
  format: yaml
  label: Xproapi Users API
  slug: xproapi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: xproapi.com
  spf: true
hosts:
- cert_expires: Dec 26 19:51:28 2026 GMT
  host: xproapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xproapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xproapi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Xproapi
provider_slug: xproapi
slug: xproapi-domain-security
source_filename: xproapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xproapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 19:51:28 2026 GMT\n  hsts: false\ndomains:\n- domain: xproapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/security/xproapi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- X
- Social
- Monitoring
- Data
---
