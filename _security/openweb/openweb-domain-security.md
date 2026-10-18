---
api_specs:
- filename: openweb-export-api-openapi.yml
  format: yaml
  label: OpenWeb Export API
  slug: openweb-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-export-api-openapi.yml
- filename: openweb-top-comments-api-openapi.yml
  format: yaml
  label: OpenWeb top comments API
  slug: openweb-top-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-top-comments-api-openapi.yml
- filename: openweb-trending-articles-api-openapi.yml
  format: yaml
  label: OpenWeb trending articles API
  slug: openweb-trending-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-trending-articles-api-openapi.yml
- filename: openweb-article-api-openapi.yml
  format: yaml
  label: OpenWeb Article API
  slug: openweb-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-article-api-openapi.yml
- filename: openweb-comment-api-openapi.yml
  format: yaml
  label: OpenWeb Comment API
  slug: openweb-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-comment-api-openapi.yml
- filename: openweb-live-blog-api-openapi.yml
  format: yaml
  label: OpenWeb live blog API
  slug: openweb-live-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-live-blog-api-openapi.yml
- filename: openweb-moderation-policy-api-openapi.yml
  format: yaml
  label: OpenWeb moderation policy API
  slug: openweb-moderation-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-moderation-policy-api-openapi.yml
- filename: openweb-score-and-reviews-api-openapi.yml
  format: yaml
  label: OpenWeb score and reviews API
  slug: openweb-score-and-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-score-and-reviews-api-openapi.yml
- filename: openweb-sso-api-openapi.yml
  format: yaml
  label: OpenWeb SSO API
  slug: openweb-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-sso-api-openapi.yml
- filename: openweb-token-api-openapi.yml
  format: yaml
  label: OpenWeb Token API
  slug: openweb-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openweb.com
  spf: true
hosts:
- cert_expires: Sep  3 16:10:21 2026 GMT
  host: www.openweb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 05:42:33 2026 GMT
  host: developers.openweb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.openweb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Openweb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenWeb, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenWeb
provider_slug: openweb
slug: openweb-domain-security
source_filename: openweb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:10:21 2026 GMT\n  hsts: false\n- host: developers.openweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:42:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: openweb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/security/openweb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Community
- Comments
- Audience Engagement
- Publishing
- Media
- Moderation
- Identity
- SSO
- Webhook
---
