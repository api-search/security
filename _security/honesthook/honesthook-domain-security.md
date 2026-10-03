---
api_specs:
- filename: honesthook-bluesky-api-openapi.yml
  format: yaml
  label: HonestHook Bluesky API
  slug: honesthook-bluesky-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-bluesky-api-openapi.yml
- filename: honesthook-github-api-openapi.yml
  format: yaml
  label: HonestHook GitHub API
  slug: honesthook-github-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-github-api-openapi.yml
- filename: honesthook-history-api-openapi.yml
  format: yaml
  label: HonestHook History API
  slug: honesthook-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-history-api-openapi.yml
- filename: honesthook-instagram-api-openapi.yml
  format: yaml
  label: HonestHook Instagram API
  slug: honesthook-instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-instagram-api-openapi.yml
- filename: honesthook-linktree-api-openapi.yml
  format: yaml
  label: HonestHook Linktree API
  slug: honesthook-linktree-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-linktree-api-openapi.yml
- filename: honesthook-mastodon-api-openapi.yml
  format: yaml
  label: HonestHook Mastodon API
  slug: honesthook-mastodon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-mastodon-api-openapi.yml
- filename: honesthook-medium-api-openapi.yml
  format: yaml
  label: HonestHook Medium API
  slug: honesthook-medium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-medium-api-openapi.yml
- filename: honesthook-movers-api-openapi.yml
  format: yaml
  label: HonestHook Movers API
  slug: honesthook-movers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-movers-api-openapi.yml
- filename: honesthook-nichos-api-openapi.yml
  format: yaml
  label: HonestHook Nichos API
  slug: honesthook-nichos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-nichos-api-openapi.yml
- filename: honesthook-pinterest-api-openapi.yml
  format: yaml
  label: HonestHook Pinterest API
  slug: honesthook-pinterest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-pinterest-api-openapi.yml
- filename: honesthook-soundcloud-api-openapi.yml
  format: yaml
  label: HonestHook Soundcloud API
  slug: honesthook-soundcloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-soundcloud-api-openapi.yml
- filename: honesthook-threads-api-openapi.yml
  format: yaml
  label: HonestHook Threads API
  slug: honesthook-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-threads-api-openapi.yml
- filename: honesthook-tiktok-api-openapi.yml
  format: yaml
  label: HonestHook Tiktok API
  slug: honesthook-tiktok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-tiktok-api-openapi.yml
- filename: honesthook-trends-api-openapi.yml
  format: yaml
  label: HonestHook Trends API
  slug: honesthook-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/honesthook-trends-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: honesthook.com
  spf: true
hosts:
- cert_expires: Dec  5 15:44:48 2026 GMT
  host: honesthook.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Honesthook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HonestHook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HonestHook
provider_slug: honesthook
slug: honesthook-domain-security
source_filename: honesthook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: honesthook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 15:44:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: honesthook.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/security/honesthook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Media
- Data Aggregation
- Software-as-a-Service
---
