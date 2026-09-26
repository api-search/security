---
api_specs:
- filename: findlocal-bluesky-api-openapi.yml
  format: yaml
  label: FindLocal Bluesky API
  slug: findlocal-bluesky-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-bluesky-api-openapi.yml
- filename: findlocal-github-api-openapi.yml
  format: yaml
  label: FindLocal GitHub API
  slug: findlocal-github-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-github-api-openapi.yml
- filename: findlocal-history-api-openapi.yml
  format: yaml
  label: FindLocal History API
  slug: findlocal-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-history-api-openapi.yml
- filename: findlocal-instagram-api-openapi.yml
  format: yaml
  label: FindLocal Instagram API
  slug: findlocal-instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-instagram-api-openapi.yml
- filename: findlocal-linktree-api-openapi.yml
  format: yaml
  label: FindLocal Linktree API
  slug: findlocal-linktree-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-linktree-api-openapi.yml
- filename: findlocal-mastodon-api-openapi.yml
  format: yaml
  label: FindLocal Mastodon API
  slug: findlocal-mastodon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-mastodon-api-openapi.yml
- filename: findlocal-medium-api-openapi.yml
  format: yaml
  label: FindLocal Medium API
  slug: findlocal-medium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-medium-api-openapi.yml
- filename: findlocal-movers-api-openapi.yml
  format: yaml
  label: FindLocal Movers API
  slug: findlocal-movers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-movers-api-openapi.yml
- filename: findlocal-events-api-openapi.yml
  format: yaml
  label: FindLocal Events API
  slug: findlocal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-events-api-openapi.yml
- filename: findlocal-nichos-api-openapi.yml
  format: yaml
  label: FindLocal Nichos API
  slug: findlocal-nichos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-nichos-api-openapi.yml
- filename: findlocal-pinterest-api-openapi.yml
  format: yaml
  label: FindLocal Pinterest API
  slug: findlocal-pinterest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-pinterest-api-openapi.yml
- filename: findlocal-soundcloud-api-openapi.yml
  format: yaml
  label: FindLocal Soundcloud API
  slug: findlocal-soundcloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-soundcloud-api-openapi.yml
- filename: findlocal-threads-api-openapi.yml
  format: yaml
  label: FindLocal Threads API
  slug: findlocal-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-threads-api-openapi.yml
- filename: findlocal-tiktok-api-openapi.yml
  format: yaml
  label: FindLocal Tiktok API
  slug: findlocal-tiktok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-tiktok-api-openapi.yml
- filename: findlocal-trends-api-openapi.yml
  format: yaml
  label: FindLocal Trends API
  slug: findlocal-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-trends-api-openapi.yml
- filename: findlocal-events-api-openapi.yml
  format: yaml
  label: FindLocal Events API
  slug: findlocal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-events-api-openapi.yml
- filename: findlocal-venues-api-openapi.yml
  format: yaml
  label: FindLocal Venues API
  slug: findlocal-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-venues-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: findlocal.community
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: honesthook.com
  spf: true
hosts:
- cert_expires: Dec  4 00:13:03 2026 GMT
  host: findlocal.community
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 15:44:48 2026 GMT
  host: honesthook.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Findlocal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FindLocal, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FindLocal
provider_slug: findlocal
slug: findlocal-domain-security
source_filename: findlocal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findlocal.community\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 00:13:03 2026 GMT\n  hsts: false\n- host: honesthook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 15:44:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: findlocal.community\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: honesthook.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/security/findlocal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- API
- Hyperlocal
- Community
- Data
- OpenData
---
