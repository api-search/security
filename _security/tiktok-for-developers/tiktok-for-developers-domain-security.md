---
api_specs:
- filename: tiktok-display-openapi.yml
  format: yaml
  label: TikTok Display API
  slug: tiktok-display-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-display-openapi.yml
- filename: tiktok-content-posting-openapi.yml
  format: yaml
  label: TikTok Content Posting API
  slug: tiktok-content-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-content-posting-openapi.yml
- filename: tiktok-research-openapi.yml
  format: yaml
  label: TikTok Research API
  slug: tiktok-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-research-openapi.yml
- filename: tiktok-login-kit-openapi.yml
  format: yaml
  label: TikTok Login Kit
  slug: tiktok-login-kit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-login-kit-openapi.yml
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
