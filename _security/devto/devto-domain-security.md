---
api_specs:
- filename: devto-agent-sessions-api-openapi.yml
  format: yaml
  label: DEV Community agent_sessions API
  slug: devto-agent-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-agent-sessions-api-openapi.yml
- filename: devto-articles-api-openapi.yml
  format: yaml
  label: DEV Community articles API
  slug: devto-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-articles-api-openapi.yml
- filename: devto-billboards-api-openapi.yml
  format: yaml
  label: DEV Community billboards API
  slug: devto-billboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-billboards-api-openapi.yml
- filename: devto-comments-api-openapi.yml
  format: yaml
  label: DEV Community comments API
  slug: devto-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-comments-api-openapi.yml
- filename: devto-display-ads-api-openapi.yml
  format: yaml
  label: DEV Community display ads API
  slug: devto-display-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-display-ads-api-openapi.yml
- filename: devto-followed-tags-api-openapi.yml
  format: yaml
  label: DEV Community followed_tags API
  slug: devto-followed-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-followed-tags-api-openapi.yml
- filename: devto-followers-api-openapi.yml
  format: yaml
  label: DEV Community followers API
  slug: devto-followers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-followers-api-openapi.yml
- filename: devto-organizations-api-openapi.yml
  format: yaml
  label: DEV Community organizations API
  slug: devto-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-organizations-api-openapi.yml
- filename: devto-pages-api-openapi.yml
  format: yaml
  label: DEV Community pages API
  slug: devto-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-pages-api-openapi.yml
- filename: devto-podcast-episodes-api-openapi.yml
  format: yaml
  label: DEV Community podcast_episodes API
  slug: devto-podcast-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-podcast-episodes-api-openapi.yml
- filename: devto-profile-images-api-openapi.yml
  format: yaml
  label: DEV Community profile images API
  slug: devto-profile-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-profile-images-api-openapi.yml
- filename: devto-reactions-api-openapi.yml
  format: yaml
  label: DEV Community reactions API
  slug: devto-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-reactions-api-openapi.yml
- filename: devto-readinglist-api-openapi.yml
  format: yaml
  label: DEV Community readinglist API
  slug: devto-readinglist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-readinglist-api-openapi.yml
- filename: devto-segments-api-openapi.yml
  format: yaml
  label: DEV Community segments API
  slug: devto-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-segments-api-openapi.yml
- filename: devto-surveys-api-openapi.yml
  format: yaml
  label: DEV Community surveys API
  slug: devto-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-surveys-api-openapi.yml
- filename: devto-tags-api-openapi.yml
  format: yaml
  label: DEV Community tags API
  slug: devto-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-tags-api-openapi.yml
- filename: devto-trends-api-openapi.yml
  format: yaml
  label: DEV Community trends API
  slug: devto-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-trends-api-openapi.yml
- filename: devto-users-api-openapi.yml
  format: yaml
  label: DEV Community users API
  slug: devto-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-users-api-openapi.yml
- filename: devto-videos-api-openapi.yml
  format: yaml
  label: DEV Community videos API
  slug: devto-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dev.to
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: forem.com
  spf: true
hosts:
- cert_expires: Dec 12 22:06:30 2026 GMT
  host: dev.to
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 28 22:03:49 2026 GMT
  host: developers.forem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DEV Community, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DEV Community
provider_slug: devto
slug: devto-domain-security
source_filename: devto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.to\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 22:06:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers.forem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:03:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dev.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: forem.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/security/devto-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Developer Community
- Articles
- Blogging
- Social
- Content
- Open Source
---
