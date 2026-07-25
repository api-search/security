---
api_specs:
- filename: tiktok-for-developers-oauth-api-openapi.yml
  format: yaml
  label: TikTok for Developers OAuth API
  slug: tiktok-for-developers-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-for-developers-oauth-api-openapi.yml
- filename: tiktok-for-developers-post-api-openapi.yml
  format: yaml
  label: TikTok for Developers Post API
  slug: tiktok-for-developers-post-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-for-developers-post-api-openapi.yml
- filename: tiktok-for-developers-research-comments-api-openapi.yml
  format: yaml
  label: TikTok for Developers Research Comments API
  slug: tiktok-for-developers-research-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-for-developers-research-comments-api-openapi.yml
- filename: tiktok-for-developers-research-social-api-openapi.yml
  format: yaml
  label: TikTok for Developers Research Social API
  slug: tiktok-for-developers-research-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-for-developers-research-social-api-openapi.yml
- filename: tiktok-for-developers-research-users-api-openapi.yml
  format: yaml
  label: TikTok for Developers Research Users API
  slug: tiktok-for-developers-research-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-for-developers-research-users-api-openapi.yml
- filename: tiktok-for-developers-research-videos-api-openapi.yml
  format: yaml
  label: TikTok for Developers Research Videos API
  slug: tiktok-for-developers-research-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-for-developers-research-videos-api-openapi.yml
- filename: tiktok-for-developers-user-api-openapi.yml
  format: yaml
  label: TikTok for Developers User API
  slug: tiktok-for-developers-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-for-developers-user-api-openapi.yml
- filename: tiktok-for-developers-video-api-openapi.yml
  format: yaml
  label: TikTok for Developers Video API
  slug: tiktok-for-developers-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-for-developers-video-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tiktok.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tiktokapis.com
  spf: false
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.tiktok.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: developers.tiktok.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: open.tiktokapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiktok For Developers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TikTok for Developers, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TikTok for Developers
provider_slug: tiktok-for-developers
slug: tiktok-for-developers-domain-security
source_filename: tiktok-for-developers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiktok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.tiktok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: open.tiktokapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tiktok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tiktokapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/security/tiktok-for-developers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Analytics
- Authentication
- Content
- Social Media
- Video
---
