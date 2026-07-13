---
api_specs:
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Upload Video API
  slug: upload-post-upload-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Upload Photos API
  slug: upload-post-upload-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Upload Text API
  slug: upload-post-upload-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Profiles and Users API
  slug: upload-post-profiles-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Analytics API
  slug: upload-post-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upload-post.com
  spf: true
hosts:
- cert_expires: Sep  8 11:47:12 2026 GMT
  host: www.upload-post.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 11:47:12 2026 GMT
  host: docs.upload-post.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 14:50:07 2026 GMT
  host: api.upload-post.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upload Post Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upload-Post, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Upload-Post
provider_slug: upload-post
slug: upload-post-domain-security
source_filename: upload-post-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upload-post.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:47:12 2026 GMT\n  hsts: false\n- host: docs.upload-post.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:47:12 2026 GMT\n  hsts: false\n- host: api.upload-post.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:50:07 2026 GMT\n  hsts: false\ndomains:\n- domain: upload-post.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/security/upload-post-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Media
- Publishing
- Video
- Content
- Cross Posting
---
