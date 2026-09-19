---
api_specs:
- filename: dev-to-webhooks-asyncapi.yml
  format: yaml
  label: Dev.to Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/asyncapi/dev-to-webhooks-asyncapi.yml
- filename: dev-to-articles-api-openapi.yml
  format: yaml
  label: dev-to Articles API
  slug: dev-to-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-articles-api-openapi.yml
- filename: dev-to-comments-api-openapi.yml
  format: yaml
  label: dev-to Comments API
  slug: dev-to-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-comments-api-openapi.yml
- filename: dev-to-followers-api-openapi.yml
  format: yaml
  label: dev-to Followers API
  slug: dev-to-followers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-followers-api-openapi.yml
- filename: dev-to-organizations-api-openapi.yml
  format: yaml
  label: dev-to Organizations API
  slug: dev-to-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-organizations-api-openapi.yml
- filename: dev-to-pages-api-openapi.yml
  format: yaml
  label: dev-to Pages API
  slug: dev-to-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-pages-api-openapi.yml
- filename: dev-to-reactions-api-openapi.yml
  format: yaml
  label: dev-to Reactions API
  slug: dev-to-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-reactions-api-openapi.yml
- filename: dev-to-tags-api-openapi.yml
  format: yaml
  label: dev-to Tags API
  slug: dev-to-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-tags-api-openapi.yml
- filename: dev-to-users-api-openapi.yml
  format: yaml
  label: dev-to Users API
  slug: dev-to-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-users-api-openapi.yml
- filename: dev-to-webhooks-api-openapi.yml
  format: yaml
  label: dev-to Webhooks API
  slug: dev-to-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-webhooks-api-openapi.yml
- filename: dev-to-display-ads-api-openapi.yml
  format: yaml
  label: Dev To Display Ads API
  slug: dev-to-display-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-display-ads-api-openapi.yml
- filename: dev-to-followed-tags-api-openapi.yml
  format: yaml
  label: Dev To Followed Tags API
  slug: dev-to-followed-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-followed-tags-api-openapi.yml
- filename: dev-to-podcast-episodes-api-openapi.yml
  format: yaml
  label: Dev To Podcast Episodes API
  slug: dev-to-podcast-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-podcast-episodes-api-openapi.yml
- filename: dev-to-profile-images-api-openapi.yml
  format: yaml
  label: Dev To profile images API
  slug: dev-to-profile-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-profile-images-api-openapi.yml
- filename: dev-to-reading-list-api-openapi.yml
  format: yaml
  label: Dev To Reading List API
  slug: dev-to-reading-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-reading-list-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: forem.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dev.to
  spf: true
hosts:
- cert_expires: Oct 27 21:14:18 2026 GMT
  host: developers.forem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 22:06:30 2026 GMT
  host: dev.to
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Dev To Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dev To, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dev To
provider_slug: dev-to
slug: dev-to-domain-security
source_filename: dev-to-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.forem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 21:14:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.to\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 22:06:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: forem.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dev.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/security/dev-to-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Developer Community
- Content
- Publishing
- Social
- Blogging
- Open-Source
- Articles
- Webhook
---
