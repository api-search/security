---
api_specs:
- filename: google-blogger-blogs-api-openapi.yml
  format: yaml
  label: Google Blogger Blogs API
  slug: google-blogger-blogs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-blogger/openapi/google-blogger-blogs-api-openapi.yml
- filename: google-blogger-users-api-openapi.yml
  format: yaml
  label: Google Blogger Users API
  slug: google-blogger-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-blogger/openapi/google-blogger-users-api-openapi.yml
- filename: google-blogger-comments-api-openapi.yml
  format: yaml
  label: Google Blogger Comments API
  slug: google-blogger-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-blogger/openapi/google-blogger-comments-api-openapi.yml
- filename: google-blogger-pages-api-openapi.yml
  format: yaml
  label: Google Blogger Pages API
  slug: google-blogger-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-blogger/openapi/google-blogger-pages-api-openapi.yml
- filename: google-blogger-posts-api-openapi.yml
  format: yaml
  label: Google Blogger Posts API
  slug: google-blogger-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-blogger/openapi/google-blogger-posts-api-openapi.yml
- filename: google-blogger-blog-user-infos-api-openapi.yml
  format: yaml
  label: Google Blogger Blogger Blog User Infos API
  slug: google-blogger-blog-user-infos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-blogger/openapi/google-blogger-blog-user-infos-api-openapi.yml
- filename: google-blogger-page-views-api-openapi.yml
  format: yaml
  label: Google Blogger Blogger Page Views API
  slug: google-blogger-page-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-blogger/openapi/google-blogger-page-views-api-openapi.yml
- filename: google-blogger-post-user-infos-api-openapi.yml
  format: yaml
  label: Google Blogger Blogger Post User Infos API
  slug: google-blogger-post-user-infos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-blogger/openapi/google-blogger-post-user-infos-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: www.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Blogger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Blogger, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Blogger
provider_slug: google-blogger
slug: google-blogger-domain-security
source_filename: google-blogger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-blogger/security/google-blogger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blogging
- CMS
- Comments
- Google
- Pages
- Posts
- Publishing
---
